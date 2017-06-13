
Continuous Integration
 

Continuous integration is the practice of constantly merging development work with a Master/Trunk/Mainline branch so that you can test changes and test that those changes work with other changes.  The idea here is to test your code as often as possible so you can catch issues early on.  In the continuous integration process, most of the work is done by an automated tests technique which requires a unit test framework.  It is best practice to have a build server designed specifically for performing these tests so your development team can continue merging requests even while tests are being performed.

Continuous Delivery
 

Continuous delivery is the continual delivery of code to an environment once the developer feels the code is ready to ship - this could be UAT, staging or production.  The idea behind continuous delivery is that you’re constantly delivering code to a user base, whether it be QA or directly to customers for continual review and inspection.  Although similar to continuous integration, continuous delivery differs because it can feed business logic tests where unit tests are unable to catch all business logic, particularly design issues. In this process, you may also be delivering code for code review which may be batched for release or not until after the UAT or QA is done.  

The basis of continuous delivery is to have small batches of work continually fed to the next step so it can be consumed more easily and issues can be found early on.  This process is typically is easier for developers because issues come to light before the task has left their memory.

Continuous Deployment
 

Continuous deployment is the deployment or release of code to production as soon as it’s ready.  There is no large batching in staging nor a long UAT process before production.  Any testing is done prior to merging to the Mainline branch and is performed on production-like environments.  The production branch is always stable and ready to be deployed by an automated process.  The automated process is key because it should be able to be performed by anyone in a matter of minutes (preferably by the press of a button).  After a deploy, logs must be inspected to determine if your key metrics are affected, positively or negatively.  Some of these metrics may include revenue, user sign-up, response time or traffic and preferably these metrics are graphed for easy consumption.  


Step 1:  Developer checks in code to development branch.

Step 2: Continuous integration server picks up the change, merges it with Master/Trunk/Mainline, performs unit tests and votes on the merge to staging environment based on test results.

Step 3. If Step 2 is successful, developer deploys it to the staging environment and QA tests the environment.

Step 4. If Step 3 passed, you vote to move to production and the continuous integration server picks this up again and determines if it’s ok to merge into production.

Step 5. If Step 4 is successful, it will deploy to production environment.  


![1](https://puppet.com/sites/default/files/2016-09/puppet_continuous_diagram.gif)


https://blog.assembla.com/hs-fs/hub/365/file-1239046021-png/images/cd_process_diagram-resized-600.png?t=1497289412595&width=933&height=498&name=cd_process_diagram-resized-600.png
