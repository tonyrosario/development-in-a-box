### Dev in a Box
One of the most frustraiting parts of starting a new project is getting an environment to start with. In this vain we have decided to start a project that will give you the bare minimum to start doing java dev that in a standard way. This is in no way the only way to set up en environment, but is an easy way and hopefully enough for you to get started with development vs setting up a system for testing. 

Each of the roles can be removed from the vm by removing them from `site.yml`. If you want to do more major changes, I would recommend that you look at Ansibles [documentation](http://docs.ansible.com/). It is pretty good and simple. We try to keep the setup simple. But when you start working on the project and need more that what we are offering please fork this and make it your own.

Each role will have a `README.markdown` to describe what is done in this module and any variables that are used. It should also contain any examples of alternitives should someone want to build a new env from this.

This git repo is ment to be small, so it can be pulled down easly and not contain artifacts that are best served in other places. Please follow the following steps to download the tools that are needed. In the future this will be a script that is runnable.

##### Download the nessicary tools

    wget --no-check-certificate --no-cookies - --header "Cookie: oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/7u51-b13/jdk-7u51-linux-x64.rpm -O roles/java/files/jdk-7u51-linux-x64.rpm

    wget https://services.gradle.org/distributions/gradle-1.11-all.zip -O roles/java/files/gradle-1.11-all.zip
    
    wget https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.53/bin/apache-tomcat-7.0.53.tar.gz -O roles/tomcat/files/apache-tomcat-7.0.53.tar.gz
