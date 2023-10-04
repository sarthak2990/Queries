# Queries

```Technical Testing Experience:```
- Can you describe a challenging technical testing problem you faced in your previous role and how you resolved it?
  1. Yes in my previous project I was required to test hardware which renders video just like setup box in different video formats, so testing team use to test it manually and testing and covereing all the formats use to take 30 days of regression cycle, so I automated this complete  cycle using capture card , python and opencv so created a framework to automate thsi process and after it was done full test automation use to take 3 hours to test everything.
  2. While working in adtech company, I was required to provide a solution to calculate ad density in all the pages(total 200 diff pages) which needs to be used by PM, Ba and content team also, so I created a chrome plugin using JS for them which just need to install on chrome browser and single click use to give the output

```CI/CD Pipeline Configuration:```
- Provide an example where you configured a CI/CD pipeline using multiple technologies. What challenges did you encounter, and how did you overcome them? What technologies did you use?
  All my automation test runs on jenkins , where we create paramterised, dependent, scheduled and pipeline where we integrate our code from git , maven , allure plugins on different platforms like win , mac and the slave machine are hosted on aws servers or openstack machines 

```Infrastructure as Code:```
- Explain your experience with infrastructure as code. Can you provide an example of a project where you utilized infrastructure as code principles effectively?
 We have dockerised our project for implementation


```Version Control Systems/Repos:```
- Describe your experience working across multiple version control systems/repos. How do you handle code conflicts and ensure version control integrity in a team setting? What version control software have you used?
  To hadnle thsi we folloe forked repo system or sometime feature branch where we work and then merge it to develop branch of our code repo. I have used git primarly thru github or bitbucket and in my previous project I have used svn. To handle code conflict we try to cut fresh branch with latest branch and in team we make sure whenever we raise a new PR we will have latest pull with our develop branch and also we have created a checks in PR like 2 reviews are mandatory

```Microservices and Cloud Technologies:```
- Share an example of a project you worked on where you worked extensively with microservices and cloud-based technologies. What were the key challenges, and how did you address them?
In my project of cars24 we have very complex microservice archtietcure and testing them was very difficult due to contract changes and other network isseus, so we implemented contract tests using pact python to handle this cases. Also integration testing was also a challanges to we utilised karate framework there to automate services fast and easily mock them and also performance test them

```Performance Testing:```
- Discuss your experience in performance testing using tools like JMeter, Artillery, K6, Gatling, etc. Can you share a performance testing success story from your past projects?
  In my previous project we have migrated our php based rest api to java so we have test there performce using jmeter and also I have used gatling performace test integrated with my test created on karate framework.

```Log Tracing and Monitoring:```
- Explain your proficiency in tracing logs for applications and monitoring using tools like Grafana, Instana, Kubernetes clusters, Dynatrace, etc. How do you analyze log data to identify issues?
  I have used AWS cloud watch , splunk recently to monitor log and analyytics also we have inbuild tool for log which is build on tomcat so any error we read logs to debug what kind of issue and root cause where exactly the issue have come from. 
  also I have used Dynatrace in my previous project

```Test Automation:```
- Detail your experience with test automation, including API, data, mobile, and web automation. Can you share an example of a complex automation scenario you handled?
I have various experience of testing tools for web I have used Selenium and cypress using java , javascripot and python  with framework like testng, junit, cucumber and pytest
For mobile I have used appium with java with cucumber and testng
for API I have used multiple tools like karate , httpclient, restassured , python and cypress
for Data I have experience in automation using java and google nalytic api to fetch different analytic events and data 
Few years back I also tried pact-python to have contract tests for our webservices
I have experience in also writing shell scripts and bat scriupts to automate system level tasks

Complex scenerio handled is one of the video automation which I have mentioned earlier also there is one adtech prodcut which we required to automated using selenium we had, the main issue was on the web app whenever it got refreshed it all ui elements gets changes everytime so how I handled it by creating locators on real time from fetching its page source before tests and by using regex patterns I got the upodated locaotrs.
also in my one of my  project there was lot of dependcect on third party services so to test it thru automation we used lots of mock and stub to test our modules

```System Architecture and Programming Languages:```
- Describe your understanding of system architecture. Also, which programming languages are you proficient in?
 System architexture 
 I have experience in working with 3 different design patterns singleton , factory and POM and mostly I try to implement these whenver I have to design any framework dependeing on requirements, I am proficient in Java but also write code on python and js of core level

```Database Experience:```
- Discuss your experience using SQL and No-SQL databases. Do you have experience using in Memory DB?
I have experience in my sql and mongodb , cassandra though I feel am not expert on writing big queries, I rate myself very avergae in DB queries
I have not used Memory though I read about it and found it very interesting

```Shift-Left Testing and Test Automation Pyramid:```
- Explain your knowledge and experience with concepts like "Shift-Left Testing" and the "Test Automation Pyramid." How have you implemented these concepts in your testing approach?
 In my current team we follow shift left testing , where we are introduced early during our sprint cycle, it is like qa and dev sits with PM for requirement analysis and we start writing test(manual, automated or unit) with dev period and continously provide feedback to the dev and product team. Dev also test the features while devloping mostly by the test provided by Qa and sometime by themself

 for Automation we follow Test automation pyramis in most of my projects , so we have sets of unit, integration , api and UI tests so whenever a PR is merged from dev end our unit tests executes once it is sucess we executes our integration tests, we try to have 70% coverage on this part. after that on ce build is ready for QA we execute our api tests and smoke before moving into regression ui bigs test, by doing this we have very less depencecy on e2e test

```Networking and Its Impact on Apps/APIs:```
- Describe your understanding of networking and its intricacies concerning app and API behavior. Can you provide an example of a situation where networking issues affected the performance of an application or API?
 I feel it is very important part as recently we have faced one issue where due to slowness of network one of out ims api which use to bring user token was breaking and the consumer service  which was using those token have some time fix for fetching token after that it fails which causes one the panel in our application to popup error messages regarding unauthorised user. in this case there was no retry or failsafe was there so it would only work if user refresh the page, now it is fixed

 that is why i believe testing api behavior with different speed and error codes is very important, I beleieve it is more important then ui testing first
