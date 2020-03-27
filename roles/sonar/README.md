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

variable             example          description
sonar_version        6.4.7            Version of sonarqube server you wish to install       
sonar_db_user        sonar            User that will be created in postgresdb for sonar to connect using
sonar_db_name        sonar_db         DB that sonarqube server will connect to in postgres db
sonar_db_password    S0n14pSsw3d      Password for username crated above (should be a strong password)
sonar_web_host       0.0.0.0          bind host for sonarqube server
sonar_web_port       9000             bind port for sonarqube server
sonar_group          ec2-user         Linux user that will own the installation directory/location on filesystem
sonar_username       ec2-user         Linux group that will own the installation directory/location on filesystem
java_path            "/bin/java"      JAVA binary location on VM, can be found using "which java"
sonar_path           "/mnt"           Directory/Mountpoint where Sonarqube will be installed on FileSystem

Author Information
------------------

Yugal Arora
