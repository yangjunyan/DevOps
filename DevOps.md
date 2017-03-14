# What Is a DevOps Engineer?
A major part of adopting DevOps is creating a better working relationship between development and operations teams. Some suggestions to do this include sitting the teams together, involving them in each other's processes and workflows, and even creating one cross-functional team that does everything. In all these methods, Dev is still Dev and Ops is still Ops. 

The term DevOps Engineer tries to blur this divide between Dev and Ops and suggests that the best approach is to hire engineers who can be excellent coders as well as handle all the Ops functions. 

In short, a DevOps engineer can be a developer who can think with an Operations mindset and has the following skillset:

* Familiarity and experience with a variety of Ops and automation tools. 
* Great at writing scripts.
* Comfortable with dealing with frequent testing and incremental releases.
* Understanding of Ops challenges and how they can be addressed during design and development.
* Soft skills for better collaboration across the team.

# How Can You Be a Great DevOps Engineer?
The key to being a great DevOps Engineer is to focus on the following:

* **Know the basic concepts of DevOps** and get into the mindset of automating almost everything.
* **Know about different DevOps tools** like AWS, GitHub, Puppet, Docker, Chef, New Relic, Ansible, Shippable, JIRA, Slack, etc.
* **Have an organization-wide Ops mindset.** There are many common Ops pitfalls that developers need to consider while designing software. Reminding developers of these during design and development will go a long way in avoiding these altogether rather than running into issues and then fixing them. Try to standardize this process by creating a checklist that is part of a template for design reviews.
* **End-to-end collaboration** and helping others solve issues are key.
* **You should be a scripting guru** — Bash, Powershell, Perl, Ruby, JavaScript, Python, you name it. You must be able to write code to automate repeatable processes.


# Set the Assembly Line Up
![1](https://cloudonaut.io/images/2017/01/aws-velocity.png)

# Software Assembly Line
A typical assembly line in my projects looks like this:

* Kanban board to plan work and visualize work in progress (i.e., Trello).
* Developer environment.
  * Editor.
  * Local build.
  * Local test.
* The CI/CD pipeline.
  * Code repository (AWS CodeCommit).
  * Artifact repository (Amazon S3, Amazon EC2 Container Registry).
* Pipeline (AWS CodePipeline).
  * Build and test (AWS CodeBuild).
  * Deploy acceptance environment (AWS CloudFormation).
  * Run acceptance tests (AWS CodeBuild).
  * Deploy production environment (AWS CloudFormation).
* Monitoring (AWS CloudWatch).
  * Logging.
  * Metrics.
  * Alerting.


Docker Adoption Pathway - Part 1
https://dzone.com/articles/docker-adoption-pathway-part-1

Docker Adoption Pathway - Part 2
https://dzone.com/articles/docker-adoption-pathway-part-2

Docker Adoption Pathway - Part 3
https://dzone.com/articles/docker-adoption-pathway-part-3

Docker Adoption Pathway: Part IV
https://dzone.com/articles/docker-adoption-pathway-part-4


# Continuous Integration
## Advantages and Disadvantages of Continuous Integration
### These are some of the advantages of continuous integration:
* You catch build breaks early on.
* In a distributed development environment where developers do not always communicate with one another, continuous integration is a great way to assure the developer that the build he or she is building is the latest one.
* Continuous integration also causes less regression
* The feedback loop is smaller.
* A developer does not have to wait for the end of the day or week to find out how the check-in affected the build.
* Integration testing moves up in the chain.
* Every check-in goes through the integration testing where problems are caught early.
* Continuous integration enforces better development processes.
* Each developer is held accountable.
* You always have a latest-and-greatest build to use in demos, showcases, etc.

### On the other hand, there are some disadvantages:
* Maintenance overhead often increases.
* Some teams find that the level of discipline required for continuous integration causes bottlenecks. * This often requires a shift in the developer mindset.
* The immediate impact of a check-in often causes a backup because programmers cannot check in partially completed code.



### Recommendations for Checking In Code
The following procedure shows the recommended steps to check code into source control.
To check in code to source control
1. Verify that the CI build is working and passing all the unit tests. If it is not, notify the development lead. Do not check in code until the issue is resolved.
2. Test all code modifications in a local development environment. Make sure that the unit tests are passing.
3. Get the latest code from source control. Resolve any merge conflicts.
4. Verify that the unit tests are still passing in the local development environment.
5. Check in the modified files. There should be no merge conflicts because you synchronized them in step 3.
6. Review the code for missing comments while the CI build is running. After the CI build completes and passes all the unit tests, you can move on to next task. If the CI build fails, fix the issue because you are now blocking other developers from integrating their code.


* [Monitoring in the DevOps Pipeline](https://insights.sei.cmu.edu/devops/2015/12/monitoring-in-the-devops-pipeline.html)

* [SecDevOps: Embracing the Speed of DevOps and Continuous Delivery in a Secure Environment](https://securityintelligence.com/secdevops-embracing-the-speed-of-devops-and-continuous-delivery-in-a-secure-environment/)
* [Continuous Security: Implementing the Critical Controls in a DevOps Environment](https://www.sans.org/reading-room/whitepapers/critical/continuous-security-implementing-critical-controls-devops-environment-36552)

* [7 cool tools for doing devops right](http://www.infoworld.com/article/2866574/devops/7-cool-tools-for-doing-devops-right.html#)
* [Why “Enterprise DevOps” Doesn’t Make Sense](https://devops.com/enterprise-devops-doesnt-make-sense/)
* [Understanding Docker, Containers and Safer Software Delivery](https://www.sitepoint.com/docker-containers-software-delivery/)
* [8 more cool tools for devops success](http://www.infoworld.com/article/3031009/devops/8-more-cool-tools-for-devops-success.html)

https://www.cloudbees.com/sites/default/files/jenkins2-harpreet-blog2-1.png
http://cdn.electric-cloud.com/wp-content/uploads/sdlc-tools.jpg

https://devops.com/wp-content/uploads/2015/04/cd-devops.png

http://www.adventone.com.au/wp-content/files_mf/1460512945Devopsfordummies.pdf
https://devops.com/31-reference-architectures-devops-continuous-delivery/

# Free Course
* [Introduction to DevOps: Transforming and Improving Operations](https://www.edx.org/course/introduction-devops-transforming-linuxfoundationx-lfs161x)


What DevOps Is and What It Is Not
https://dzone.com/articles/what-devops-is-and-is-not

 Its core values are Culture, Automation, Lean, Measurement and Sharing (CALMS).
http://www.ranger4.com/ranger4-devops-blog/i-got-devops-certified

Why Continuous Delivery Is Key for Developer Career Success
https://dzone.com/articles/why-continuous-delivery-is-key-for-developer-caree
