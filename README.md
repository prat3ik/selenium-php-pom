# Selenium - PHPUnit Example Project with Page Object Model
---
### How to use?

Create the Page Objects of your Web application under **_pageobjects_** package, call those Page Objects in  [PHPUnit](https://phpunit.de/) tests under **_tests_** package (Sample Page Objects, testcase included in this template)

### How to setup(Mac)?
1) Make sure PHP is installed.
2) install composer using: `$ brew install composer`
3) Move to Project directory.
4) Install project dependencies using command: `$ composer update`, After successfully installing this you can observe that **vendor** directory will be created in project root directory.
5) Install Standalone Selenium Jar from: https://www.seleniumhq.org/download/
6) Download latest version of WebDriver binary, for example chromedriver binary from: http://chromedriver.chromium.org/
7) Start Selenium server with required WebDriver binaries, for example with chromedriver binary: `$ java -Dwebdriver.chrome.driver=/path/to/chromedriver -jar /path/to//selenium-server-standalone.jar`
8) Check Selenium server is up and Running on: http://localhost:4444/
9) Execute test cases(Mentioned on Test.php, and make sure you are at root of project directory which by default you are as you have follwed above steps): `$ ./vendor/bin/phpunit tests`

By default it runs in Chrome browser, you can specify which browser to use as well like `$ ./vendor/bin/phpunit tests firefox`

Browsers added in this template are 
* chrome
* firefox
* ie
* opera
* edge
* safari
* phantomjs

> Feel free to modify it to your own needs :)
