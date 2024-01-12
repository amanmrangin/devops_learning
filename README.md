# devops_learning
**DevOps** is a set of practices that combines software **Dev**elopment and IT **Op**erations, aims to shorten the SDLC and provide Continuous Delivery with quality. A successful DevOps implementation is achieved by set of Tools in following phases.
  #### Phases of Dev: 
  ### Plan
  ### Code: GitHub, BitBucket
  ### Build: 
  ### Test : Build Test
  #### Phases of Ops:
  ### Release
  ### Deploy
  ### Operate
  ### Monitor
  #### DevOps Processes:
   ##### Continuous Delivery (CD)
   ###### Continuous Integration (CI)
     A Process for
      - All Developers to
        -- Commit the source code and unit test cases into branches of Git Repository of SCM/VCS tools such as GitHub, BitBucket
        -- Create Pull Request to review the code
        -- Approve Pull Request and Merge and Push the code into uch as GitHub or BitBucket etc
      - CI servers such as Jenkins, TeamCity, CircleCI, GitHub Actions, BitBucket Pipeline, TravisCI 
        -- Pull the sourcode from branch(es) of Git Repo, 
        -- Run **build** tools such as Maven, Ant, Grails, to **compile**, **run unit test-cases**, **run integration-tests**
        -- Run Code Analysis tools (Sonar, JFrog's XRay) to verify the quality of source code for programming standards, CodeCoverage by Unit Testcases, Scan for Vulnerabilities
  ##### Continuous Build
  ##### Continuous Deployment
    - A process to
      -- Build the infrastructure of an environment(s) using configuration file consisting of Java versions, JVM Agent(s) , servers (Tomcat/Websphere)
      -- Deploy the  **code (artifact)**, external application-specific configuration (.properites, secrets, keys, certs etc) into target environments
  ##### Continuous Release 
 
    - A process to automatically 
      -- create the **packaged** artifact (.jar, .war. ear), 
      -- Save/push into a **Artifactory Server** (e.g. JFrog Artifactory, Nexus, Trusted Repository)
      -- **deploy** the artifact into a target environment(s)
    
    
    

