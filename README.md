Welcome to the AWS CodeStar sample web application
==================================================

This sample code helps get you started with a simple Express web application
deployed by AWS Elastic Beanstalk.

What's Here
-----------

This sample includes:

* README.md - this file
* .ebextensions/ - this directory contains the configuration files that
  AWS Elastic Beanstalk will deploy your Express application
* package.json - this file contains various metadata relevant to your Node.js
  application such as dependencies
* server.js - this file contains the code for your application
* public/ - this directory contains static web assets used by your application
* tests/ - this directory contains unit tests for your application


Getting Started
---------------

These directions assume you want to develop on your local computer, and not
from the Amazon EC2 instance itself. If you're on the Amazon EC2 instance, the
virtual environment is already set up for you, and you can start working on the
code.

To work on the sample code, you'll need to clone your project's repository to your
local computer. If you haven't, do that first. You can find instructions in the
AWS CodeStar user guide.

1. Install Node.js on your computer.  For details on available installers visit
   https://nodejs.org/en/download/.

2. Install NPM dependencies:

        $ npm install

3. Start the development server:

        $ node server.js

4. Open http://127.0.0.1:3000/ in a web browser to view your application.

What Do I Do Next?
------------------

Once you have a virtual environment running, you can start making changes to
the sample Express web application. We suggest making a small change to
/public/index.html first, so you can see how changes pushed to your project's
repository are automatically picked up and deployed to the Amazon EC2 instance
by AWS Elastic Beanstalk. (You can watch the progress on your project dashboard.)
Once you've seen how that works, start developing your own code, and have fun!

To run your tests locally, go to the root directory of the 
sample code and run the `npm test` command, which
AWS CodeBuild also runs through your `buildspec.yml` file.
 
To test your new code during the release process, modify the existing tests or 
add tests to the tests directory. AWS CodeBuild will run the tests during the 
build stage of your project pipeline. You can find the test results
in the AWS CodeBuild console.
 
Learn more about AWS CodeBuild and how it builds and tests your application here:
https://docs.aws.amazon.com/codebuild/latest/userguide/concepts.html

Learn more about AWS CodeStar by reading the user guide.  Ask questions or make
suggestions on our forum.

User Guide: http://docs.aws.amazon.com/codestar/latest/userguide/welcome.html

Forum: https://forums.aws.amazon.com/forum.jspa?forumID=248
