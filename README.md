# Playwright-Javascript-SeleniumGrid
Playwright Automated Test cases integrated with Selenium Grid Docker
## **** HOW TO RUN PLAYWRIGHT TEST CASES IN SELENIUM GRID DOCKER FROM JENKINS **** ##
<ul>
  <li> Create a docker-compose file in the root directory
  <li> Trigger the docker-compose file with the below command:
  
        
        docker-compose up -d
        
  <li> Once the containers are up, navigate to localhost:4444 and check selenium grid UI is showing or not
  <li> Now, Build a Job in jenkins and connect the git repo
  <li> Monitor your test cases being executed through the Selenium Grid sessions VNC viewer
  <li> Password for the VNC viewer is:
  
  ```
  secret
