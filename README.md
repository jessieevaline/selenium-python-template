# Template: Selenium Testing with Python

## Instructions

This is a template repository:
It means that you can create your own repository from this template with the same files and folder structure.

To create your own repository find the button "Use this template" above the file list and click it.
You will be asked to give your repo a name (but you can also use the name of the template, as the new repo will be created in your own Github account).
You can also chose from the same options as if you were creating a new repository from scratch.

For detailed instructions with screen shots check out the [Github docs](https://docs.github.com/en/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template).

After you have created your own repository, you are ready to get started with the next steps below!


### Set up Webdriver for Selenium with Firefox

To allow your application to control the browser you need to have browser-specific WebDriver binaries installed.

**This won't work on Windows unfortunately**
Selenium works with a range of different browsers. The inital test in this project uses Firefox.

Go to the [Downloads Page for Geckodriver](https://github.com/mozilla/geckodriver/releases) and select the latest versin for your Operating System.

Download the right version of Geckodriver and move it to the `webdriver` folder of this project.

When you are running the tests, you will have to add this folder to the $PATH variable to make it available for the application.
You can copy the whole command including the PATH from below.

### Set up Webdriver for Selenium with Chrome

Go to the [Downloads Page for Chromedriver](https://chromedriver.chromium.org/downloads) and select the appropriate version for your Chrome Installation and Operating System.

Download the right version of Chromedriver and move it to the `webdriver` folder of this project.
As the example test is using Firefox, you will have to adjust it to work with Chrome as well.
The command to run the tests works the same way for both browsers, so you can again copy it from below.

## Set up all other libraries

We will also need the `selenium` library to run the test code.

You can install it with:
```
pip install selenium
```

This will download the library with the bindings for [selenium](https://pypi.org/project/selenium/).


### Run the example Test

After you have installed and downloaded everything we need, you are ready to execute the example test.
Run the following command in your console:
```
PATH=$PATH:`pwd`/webdriver python -m unittest
```

This will execute all test files in `/test` - in this case only the example test file.
You should see the browser start, navigate to a website and also the output from the successful test run in the console.


## Add your own tests!

Create new files in the `/tests` folder for your own test cases. Note that all test files should start with `test_`.
You can use the existing test as the basis.

To learn more about the commands to control the Browser with selenium, check the [Python docs for Selenium](https://www.selenium.dev/selenium/docs/api/py/api.html).
There is also a Tutorial on [Browser Manipulation](https://www.selenium.dev/documentation/en/webdriver/browser_manipulation/) in different programming languages.

If you need more info about creating tests in python with the unittest library, check the [docs for unittest](https://docs.python.org/3/library/unittest.html).