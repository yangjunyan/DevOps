# Continuous Integration

# 5 Best Practices in Continuous Integration
Continuous Integration is the first stepping stone in Continuous Delivery Pipeline. Automating testing through Continuous Integration improves code quality. Implemented with best practices, CI helps in getting early feedback, increases transparency and sets the stage for better Continuous Delivery thus improving DevOps maturity. Following are a few best practices for implementing a successful CI practice:

1. Manage Source Code:
* **Centralized version control repository:** Source code should be managed using centralized version control repository.
* **Code Review:** Two levels of Code Review must be performed.
* **Compile, Unit Test and Static Code Analysis:** Code should be Built, Unit tested, and Analyzed using Static Code Analysis tools before pushing to the central repository.
* **Code Commit:** Code changes must be pushed to central repository multiple times a day or at least once a day to the main line.

2. Manage Software Binaries:
* **Binary Repository Manager:** Software Binaries must be centralized using the Binary repository manager, and software dependencies between teams must be seamlessly shared.
* **Vulnerabilities and Compliance:** Software Binaries must be scanned for security vulnerabilities and license compliance. The build should be failed if vulnerabilities are found in software binaries.
* **Publish Builds:** Build artifacts should be published to a Binary repository to be able to share seamlessly with dependent module builds.
* **Deployment Automation:** Deployment of build artifacts to environments should happen from the binary repository for better security and reliability.

3. Build Automation:
* **VCS Trigger:** Builds must be triggered for every code change done in source control repository.
* **Unit Tests and Static Code Analysis:** Static Code Analysis and Unit Tests must be run for every check-in.
* **CI Job as code:** Build configuration must be maintained as the code.
* **Feedback:** Notifications must be sent to developers on build failures, SCA criteria not met, and Unit Tests Failure, Security Vulnerabilities, and License Compliance.

4. Reduce Build Time:
* **Modularizing code and Micro Services:** Independently buildable components must be identified and the builds simplified by executing them in smaller sizes to minimize the Build time.
* **Dependency Management:** Binaries from Binary Repository Manager setup must be resolved behind the company firewall to reduce the time taken to download from external portals.
* **Collocation of machines and repositories:** Build machines, source code repository and Binary repository must be collocated – this creates the least network latency for pulling source code and Binaries.

5.Automate Deployment and Tests:
* **Automated Environment:** Environment Provisioning and Configuration management using tools with code from Version control repository must be used.
* **Deployment Automation:** Deployment must be automated by identifying simple steps, configuring entire workflows, and implementing the flow using script or tool.
* **CI Build Tested:** The CI Build must be self-tested in a production like environment.

# 5 Top Tools to Build Scalable CI
Today, there are multiple tools available in the market that help build a scalable Continuous Integration practice. Following is a list of 5 well known and robust tools:

CircleCI: It is one of the SAAS-based CI servers for simple setups. CircleCI is the best CI/CD solution for teams who want to build faster, ship more, and fail less at any scale.
Go: It helps distribute builds across different systems and monitor them all at one place. It is easy to perform regular tasks as they are added to the pipeline.
Jenkins: It is developed in Java and can be installed using the simple java command: –jar Jenkins.war. It is mainly used for building and testing software projects continuously and monitoring externally-run jobs.
TeamCity: This is a powerful CI server from JetBrains for enterprise needs with high availability and scalability. A Continuous Integration server, TeamCity encompasses all the features you expect from a mature Continuous Deployment platform.
Travis CI: This is one of the simplest CI servers to get started, is available as open source, and is also free to host on your server.
5 Major Benefits of Implementing CI
5 major benefits that Continuous Integration brings to the table are:

Delivers software on time with market-readiness
Identifies issues faster and thus helps resolution in real-time
Brings to an end the need of longer and stressful integrations
Brings to an end the need to wait for evaluating if the code is functioning properly
Enhances visibility of the development process for better interaction and resolution





A typical continuous integration workflow will contain:
* Setting up the automated build and unit testing
* Setting up machines for application deployment and testing
* Configuring for application deployment and testing
* Queuing the Build, execute Tests and Test results analysis
* Configuring the whole work flow to execute on a continuous basis


# A Sample Continuous Integration Workflow
* Check in Code
* New Build Is Kicked Off
* Code Is Checked Out
* Code Is Compiled
* Static Analyzers Are Run
* Unit Tests Are Run
* Results Are Reported
* Software Is Packaged
* Code Is Optionally Deployed (Continuous Deployment)

https://dzone.com/refcardz/continuous-integration

* [5 Best Practices in Continuous Integration](http://www.cigniti.com/blog/continuous-integration-5-best-practices-best-tools-benefits/)

https://dzone.com/refcardz/continuous-integration
