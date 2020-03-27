Role Name
=========

Role for Sonarqube server installation

Requirements
------------

Role has been tested on Centos7
The only prerequisite for running SonarQube is to have Java (Oracle JRE 8 or OpenJDK 8) installed on your machine.
This ansible role manages remaining pre-requisites and dependencies
https://docs.sonarqube.org/display/SONARqube71/Requirements

Role Variables
--------------

A description of the settable variables for this role:

|   variable           |  example       |   description
|   -----------------  |  -----------   |   -----------
|   sonar-version      |  6.4.7         |   Version of sonarqube server you wish to install       
|   sonar-db-user      |  sonar         |   User that will be created in postgresdb for sonar to connect using
|   sonar-db-name      |  sonar-db      |   DB that sonarqube server will connect to in postgres db
|   sonar-db-password  |  S0n14pSsw3d   |   Password for username crated above (should be a strong password)  
|   sonar-web-host     |  0.0.0.0       |   bind host for sonarqube server
|   sonar-web-port     |  9000          |   bind port for sonarqube server
|   sonar-group        |  ec2-user      |   Linux user that will own the installation directory/location on filesystem
|   sonar-username     |  ec2-user      |   Linux group that will own the installation directory/location on filesyste
|   java-path          |  "/bin/java"   |   JAVA binary location on VM, can be found using "which java
|   sonar-path         |  "/mnt"        |   Directory/Mountpoint where Sonarqube will be installed on FileSystem  

Author Information
------------------

Yugal Arora
