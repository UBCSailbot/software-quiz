# Technical Quiz - UBC Sailbot Software

## Instructions

1. Clone this repository

2. Create a public repository

3. Change the "origin" remote to point to the repository you created: [how to change the URI (URL) for a remote Git repository](https://stackoverflow.com/a/2432799)

4. Complete the Python functions in `standard_calc.py` **or** C functions in `standard_calc.cpp`

### Python Option

5. Add PyTest unit tests in `test_standard_calc.py` to verify your implementations are correct

6. Pushing your code will run a linter and your tests.
You can find the results in the Actions tab on GitHub: [viewing your workflow results](https://docs.github.com/en/actions/quickstart#viewing-your-workflow-results).
    - To run these tests locally on your computer:
        1. Install the required packages

            ```sh
            pip install flake8 pytest
            ```

        2. Execute the following commands

            ```sh
            flake8 . --count --max-complexity=10 --max-line-length=127 --statistics
            ```

            - Outputs `0` on success

            ```sh
            pytest
            ```

7. When you are done, send us the link to your repository

### C/C++ Option
Even though the functions are defined in C++ files, you can use standard C syntax without issue. The use of .cpp files
just makes it so you can write in either C or C++.

This repository includes the [CuTest](https://github.com/ennorehling/cutest) unit test framework. It was chosen because
it is simple and supports both C and C++. The Kernel/Navigation subteam uses C++ and [GoogleTest](https://github.com/google/googletest),
so you can try using those if you want to get a hang of the tools earlier (you also get bonus points).

These are not strict instructions. You can change whatever you wish so long as the functions specifications in
`standard_calc.cpp` are met and unit tests are included.

5. Run `git submodule update --init` to pull the unit test framework.

6. Add unit tests to `test_standard_calc.cpp` to verify your implementations are correct

7. If you are on Linux, run `make` in your terminal to compile your code and `./test_standard_calc.o` to run it
   If you are on Mac, perform the same steps as Linux. If you get an error about gcc not being installed then edit the Makefile and replace gcc with clang
   If you are on Windows, you can add the files to VSCode and compile/run that way, or install a compiler like
   [MinGw](https://sourceforge.net/projects/mingw-w64/files/Toolchains%20targetting%20Win32/Personal%20Builds/mingw-builds/installer/mingw-w64-install.exe) (link is to the installer download) and do the Linux steps

8. Push your code and send us a link to your repository

## Resources

You may use any resources you find, but must complete the quiz individually.
Here are some resources to get you started:

- [Python](https://www.python.org/about/gettingstarted/)
- [PyTest](https://docs.pytest.org/en/6.2.x/getting-started.html)
- [Flake8](https://flake8.pycqa.org/en/latest/)
