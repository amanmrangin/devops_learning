# DevOps_learning

**DevOps** is a set of practices that combines software **Dev**elopment and IT **Op**erations, aims to shorten the SDLC and provide Continuous Delivery with quality. A successful DevOps implementation is achieved by set of Tools in following phases.

## Phases of Dev and Tools:
    Plan: 
        Uses a tool, JIRA, to follow the Agile practies to break down the business requirments into User Stories/Epics/Features that helps the developers to implement and testers to develop testcases to validate the implementation.
        A tool, Slack/MS Teams Channels, to communicate and collaborate between all Team members.
    Code: Allows developers and testers to write and save the sourcecode and testcases into repositories in GitHub/BitBucket.
    Build: A tool, Jenkins, with ability to integrate with any plugins/tools (Maven, Gradle, Sonar) to compile, scan, find the quality in the sourcecode.
    Test: A tool, Jenkins, to perform the automated testcases (JUnit, Selenium, TestNG) to validate the sourcecode.

## Phases of Ops and Tools:
    Release:
    Deploy:
    Operate:
    Monitor:        
        Provides **Observability** by instrumenting the systems (e.g.: Docker images, ) and applications (e.g.: Java Web) to collect the **metrics** (e.g.: NewRelic JVM Agent, DataDog JVM Agent, Contrast Access JVM Agent,) and **logs** (e.g. Splunk JVM Agent).
        The Metrics from tools provides the Quantitative data to understand how the Infrastructure of System and application is behaving and eliminates the guess.

        Splunk Log Management Tool: Allows searching in logs (syslogs, firewall logs, application-log4j, aws, database) in a centralized location (Splunk Log Server) that are collected from different sources (applications through JVM Agents, servers).
        ELK (Elastic Search, Logstash, Kibana): To Manage, Analyze, troubleshoot, gain insights from the collected log data.

        DataDog/Ciso App Dynamics/Newr Relic: Allows the technical people to search and trace 
            - Applications: requests/response, page load, availability
            - Web tracking (Google Analytics): User location, device type
            - Infrastructure (AWS CloudWatch)
            - System (CPU, Memory, Disk, Logs)            -
            - learn the system performance under Stress/Load conditions, uptime, CPU load, on/off peak usages, availability period as per Service Level Agreement.

        Notes: 
           - Expose the information enough to understand the behavior of system/applications/platforms/infrastructure
           - Transmit/collect/store the information in a centralized location
           - Mindful of the associated costs to Storage
           - Reduce the Log levels to control the flood
           - Mask/redact the sensitive data 
           - Build Alerts to create Tickets  based on events/incidents to get the attention from team(s) to respond
           - Have Root Cause Analysis (RCA) on the events

## DevOps Processes:
    
### Continuous Delivery (CD): 
    A practice that combines the practies of both Continuous Integration(CI) and Continous Deployment (CD). There are a few tools offer these practices implemented independently or combined to increase the velocity of developer by reducing the cycle time between build, test and deploy phases

        Continuous Integration (CI): A Process for
         - All Developers to
            -- Commit the source code and unit test cases into branches of centralized Git Repository of SCM/VCS tools such as GitHub, BitBucket
            -- Create Pull Request to review the code
            -- Approve Pull Request and Merge and Push the code into uch as GitHub or BitBucket etc
         - CI servers such as Jenkins, TeamCity, CircleCI, GitHub Actions, BitBucket Pipeline, TravisCI to automate the
            -- Pull the sourcecode from branch(es) of Git Repo. A pre-configured WebHook in Git (e.g.: GitHub or BitBucket) and in CI (e.g.: Jenkins) will trigger 
            -- Run build tools such as Maven, Ant, Grails, to **compile**, **run unit test-cases**, **run integration-tests**
            -- Run Code Analysis tools (Sonar, JFrog's XRay) to verify the quality of source code for programming standards, CodeCoverage by Unit Testcases, Scan for Vulnerabilities
            -- create the **packaged** artifact (.jar, .war. ear), and Save/push into a **Artifactory Server** (e.g. JFrog Artifactory, Nexus, Trusted Repository)

### Continuous Deployment (CD) : 
    A process to automatically deploy the application(s) to an environment (Non-Production Environment, Production Environment)
         - Build the infrastructure (servers, memory, load blancers, nodes etcc) of environment(s) using configuration file consisting of Java versions, JVM Agent(s) , servers (Tomcat/Websphere)
        - Deploy the  **code (artifact)**, external application-specific configuration (.properites, secrets, keys, certs etc) into target environments

### Continuous Build

### Continuous Release
    - A process to automatically
      -- create the **packaged** artifact (.jar, .war. ear),
      -- Save/push into a **Artifactory Server** (e.g. JFrog Artifactory, Nexus, Trusted Repository)
      -- **deploy** the artifact into a target environment(s)


## References
- [Maruthi Tech at Medium.com](https://marutitech.medium.com/top-12-devops-tools-for-your-devops-implementation-plan-e159e0db9ac2) 

- [Simplilearn](https://www.simplilearn.com/tutorials/devops-tutorial/continuous-delivery-and-continuous-deployment)


