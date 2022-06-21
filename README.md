# JenkinsStageTest
Creating 2  jenkins pipeline for testing

**1st pipeline - Testing  react app**

Build stage --> to pull files from github repository and then build a container image from it

run stage --> to run the container image and open port 8080 

stop stage --> to stop and delete the container

**2nd pipeline -Testing docker-compose **

Build pretest container stage --> po pull files from github repository and then build a container image from it

Pretesting stage --> npm test to run test

Curl page to check app stage --> sleep 15 seconds and test curl the localhost to ensure container build has no issue

Stop docker-compose stage --> to stop the containers
