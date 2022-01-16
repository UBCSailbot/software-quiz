# Technical Quiz - UBC Sailbot Software

## Instructions

1. Clone this repository

2. Create a public repository

3. Change the "origin" remote to point to the repository you created: [how to change the URI (URL) for a remote Git repository](https://stackoverflow.com/a/2432799)

4. Complete the Python functions in `standard_calc.py`

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

## Resources

You may use any resources you find, but must complete the quiz individually.
Here are some resources to get you started:

- [Python](https://www.python.org/about/gettingstarted/)
- [PyTest](https://docs.pytest.org/en/6.2.x/getting-started.html)
- [Flake8](https://flake8.pycqa.org/en/latest/)
