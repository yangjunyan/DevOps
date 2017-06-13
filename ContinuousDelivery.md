
Step 1:  Developer checks in code to development branch.

Step 2: Continuous integration server picks up the change, merges it with Master/Trunk/Mainline, performs unit tests and votes on the merge to staging environment based on test results.

Step 3. If Step 2 is successful, developer deploys it to the staging environment and QA tests the environment.

Step 4. If Step 3 passed, you vote to move to production and the continuous integration server picks this up again and determines if it’s ok to merge into production.

Step 5. If Step 4 is successful, it will deploy to production environment.  


![1](https://puppet.com/sites/default/files/2016-09/puppet_continuous_diagram.gif)


https://blog.assembla.com/hs-fs/hub/365/file-1239046021-png/images/cd_process_diagram-resized-600.png?t=1497289412595&width=933&height=498&name=cd_process_diagram-resized-600.png
