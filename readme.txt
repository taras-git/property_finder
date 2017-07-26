Prerequisites

Protractor is a Node.js program (please check guide https://nodejs.org/en/)
Download Protractor package using npm

NOTE:
1. To run the protracor test suite, Node v.6 is required:
    $curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
    $sudo apt-get install -y nodejs

2. Download and install jasmine-reporter tool :
    $npm install protractor-jasmine2-html-reporter --save-dev



Setup

Use npm to install Protractor globally with: $npm install -g protractor

webdriver-manager is a helper tool included in protractor.
Download the necessary binaries with: $webdriver-manager update



Running the tests

Open a new console. 
Start up a server with: $webdriver-manager start
(Hint: you may need to run $webdriver-manager update, in oder to obtain the last version of driver)
Open another console and navigate to folder where the current project conf.js file is, i.e. PropertyFinderTestProject/e2e/conf
Run the tests : $protractor conf.js --suite home,findAgent,collectAgentInfo



Test results

Test results are stored in PropertyFinderTestProject/e2e/results/ folder.
There are screenshots and HTML report (my-report.html).
Every new test run rewrites the old reports.
