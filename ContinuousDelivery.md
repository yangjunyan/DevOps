
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





https://victorops.com/blog/

https://s-media-cache-ak0.pinimg.com/736x/d2/97/4f/d2974ff1c23cb8e85d7a6d5931067653.jpg
https://s-media-cache-ak0.pinimg.com/736x/8d/cb/35/8dcb356e5df9c194057d53b3628b38f8.jpg
https://image.slidesharecdn.com/sharepointcontinuousintegrationwithvsonlineandazure-140510101655-phpapp01/95/sharepoint-continuous-integration-with-vsonline-azure-espc14-4-638.jpg?cb=1399949644
https://4.bp.blogspot.com/-L0bNvBeUJ0M/VwAwnxFmZEI/AAAAAAAABcg/kitQ5yqe3BsIprPs_E714JzVjIRPVN72w/s640/CI_CDY_CDT_04.png
https://s-media-cache-ak0.pinimg.com/736x/1d/37/3f/1d373f4905681ea155e193b1a1ed75c8.jpg
https://s-media-cache-ak0.pinimg.com/736x/ab/e4/e7/abe4e78815470248679721929891c4ba.jpg
https://s-media-cache-ak0.pinimg.com/736x/06/13/f1/0613f1a0e1af6b5c4fe0ba1df097a5f3.jpg
https://s-media-cache-ak0.pinimg.com/736x/ce/72/a8/ce72a89c3d9489b9bc80418c2008a6d3.jpg
https://s-media-cache-ak0.pinimg.com/736x/5e/38/92/5e3892c5467701035aadf7f1bbc86432.jpg


# Automating Infrastructure
http://www.rightscale.com/blog/sites/default/files/Continuous%20Integration%20and%20Continuous%20Delivery%20Best%20Practices.png
http://www.rightscale.com/blog/sites/default/files/Automating%20Infrastructure%20as%20Code%20v2.png

# 31-reference-architectures-devops-continuous-delivery
https://devops.com/31-reference-architectures-devops-continuous-delivery/


https://blog.testfort.com/testing-methodologies/4-qualities-scrum-master


* [Why to invest in Vulnerability Assessment and Penetration Testing?](http://www.cigniti.com/blog/invest-vulnerability-assessment-penetration-testing/)


* [The Growing Role of Machine Learning in Monitoring](https://logz.io/blog/machine-learning-in-monitoring/)

* [Top 5 DevOps Podcasts](https://logz.io/blog/devops-podcasts/


* [Container Security: Secure Your Enterprise Container Infrastructure](https://dzone.com/articles/container-security-lets-secure-your-enterprise-con-1)


http://www.veracode.com/blog/managing-appsec/veracode-program-managers-perspective-best-practices-scaling-appsec-program

http://blog.cutter.com/2017/06/13/blockchain-budgets-poised-to-break-out-in-2018-initiatives-to-take-off-in-3-years/



https://s-media-cache-ak0.pinimg.com/736x/76/1f/06/761f061177a4403f45bc520d52832baf.jpg
https://s-media-cache-ak0.pinimg.com/736x/c7/a0/ff/c7a0ffa76949884c6db342185821ee13.jpg
https://s-media-cache-ak0.pinimg.com/736x/76/1f/06/761f061177a4403f45bc520d52832baf.jpg
https://s-media-cache-ak0.pinimg.com/736x/38/51/64/385164054fcb197a92f320af6dadefff.jpg

https://s-media-cache-ak0.pinimg.com/736x/71/59/86/715986078c40a3dd83914e692b4de0b8.jpg


https://s-media-cache-ak0.pinimg.com/736x/8f/bb/73/8fbb731084f44cc2ada828a098e07851.jpg
https://s-media-cache-ak0.pinimg.com/736x/8f/bb/73/8fbb731084f44cc2ada828a098e07851.jpg
https://s-media-cache-ak0.pinimg.com/736x/ee/76/27/ee76274c5456190c479fb0973473a2ca.jpg
https://s-media-cache-ak0.pinimg.com/736x/e1/9d/82/e19d8214bb491acb0142d1d5f6cef529.jpg
https://s-media-cache-ak0.pinimg.com/736x/75/c6/93/75c693503b10941beeb5d6dfff4354b8.jpg

https://s-media-cache-ak0.pinimg.com/736x/8a/3f/c4/8a3fc4fa1213b59d8c0251296dbd0b18.jpg

http://agileforall.com/wp-content/uploads/2012/01/Story-Splitting-Flowchart.pdf


https://s-media-cache-ak0.pinimg.com/736x/7c/47/6d/7c476d07baa06308b20a215788b7ac16.jpg


http://aoteastudios.com/files/agile-roles-responsibilities-poster.pdf

http://www.xmind.net/m/9uVM
https://3ovyg21t17l11k49tk1oma21-wpengine.netdna-ssl.com/wp-content/uploads/2016/03/Dev-Cul-11.png
https://s-media-cache-ak0.pinimg.com/736x/02/c5/24/02c52436cecc1db65af28a8b1915092a.jpg

https://s-media-cache-ak0.pinimg.com/736x/b5/4e/c9/b54ec9428a04eba3d3c09f3e74a49c9f.jpg

https://s-media-cache-ak0.pinimg.com/736x/24/4c/04/244c0489dff30e5e3cfe06c65b868922.jpg

https://s-media-cache-ak0.pinimg.com/736x/87/0c/52/870c5218e014353156f4ddc6e8ab99a3.jpg
http://continuousdelivery.com/wp-content/uploads/2014/02/01_CD_the_idea_low-res.jpg
http://continuousdelivery.com/wp-content/uploads/2014/02/02_CD_test_strategy_low-res.jpg
http://continuousdelivery.com/wp-content/uploads/2014/02/03_CD_automated_acceptance_test_low-res.jpg
http://continuousdelivery.com/wp-content/uploads/2014/02/04_CD_managing_data_low-res.jpg

https://i.stack.imgur.com/yOofB.png
BA
https://s-media-cache-ak0.pinimg.com/736x/26/6d/55/266d55436a392f77f7a6c58631ec2859.jpg
https://s-media-cache-ak0.pinimg.com/736x/88/5f/50/885f5071b163e0820ac392685b6826cd.jpg

https://www.cloudbees.com/sites/default/files/toolchain_3.png

http://images.techhive.com/images/article/2017/05/programmable-enterprise-100720451-large.jpg
http://www.infoworld.com/article/3177293/it-management/embracing-continuous-delivery-to-power-the-programmable-enterprise.html#tk.rss_all


https://blogs.technet.microsoft.com/devops/2016/06/21/a-git-workflow-for-continuous-delivery/
