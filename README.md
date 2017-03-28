# Jenkins
![Assistanz Jenkins](http://projects.assistanz.com/github/jenkins-logo.png)  
The software development process is very much depends upon the quality of the product deliver to the customer  and the product quality depends upon the build and number of bugs . The challenge here is to track the bug and deliver the product to a customer on time . In this scenario **CICD** or **Continuous Delivery and Continuous Integration** plays significant role and the tool which helped us to achieve this is Jenkins .

In  traditional software development procedures we used to keep the files some storage and then to upload the source files to some webservers, then do testing and then deliver to customer. All the processes are time consuming and when a bug reported, we need to redo all these steps again and again until the bugs get solved out. By using Jenkins the build delivery process to multiple environments became so eazy and within a less time frame. 

We configured a centralised repository for source code with logins for each developers who is working the project. Each of them can contribute their part to the report and then finally an administrator can merge the code to main repo. The common players in repositories are svn and git. Here we are using git (gitlab). Then we need to setup servers for developers, testers, beta version or UAT and then for production server . All these servers can configure in Jenkins as ssh or scp end points with key based or password authentication. Then we need to write Jenkins Job corresponding to the build tools, which  we are using to develop and build the source code 
**Eg : Maven, Ant, Gradle etc..**

We can collect the files from git and build using any of the build tools, then will convert the files as an archive corresponding to the webservers we used to deploy the files. For example for java projects we used to build using maven or gradle. In case of Maven, we will write the pom.xml file to create the archive as .jar or .war files . Then we can move these files to each deployment servers from the centralized Jenkins server using Build pipeline or Delivery pipeline. Jenkins provides all the needed plugins and documentation to setup the whole process. It will reduce the time consumption, complexities in the build process and also will reduce the number of bugs to end customer. In short we will be able to deliver 90 to 95% clean product to the customer and his users .

# Examples

![Assistanz Jenkins](http://projects.assistanz.com/github/assistanz-jenkins-failure.png)

The above example has an error in the testing environment. So, we cannot move to next level. In this case, we can prevent the error from moving to production environment. By this, we can deliver a quality based code to production environment.

![Assistanz Jenkins](http://projects.assistanz.com/github/assistanz-jenkins-success.png)

The above example has success in the test environment. In this case, we can move to next environment without any errors. 

further queries email us.  
sales@assistanz.com  
amal@assistanz.com  
