node {
   def mvnHome
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/prajnadnayak/java-maven-junit-helloworld.git'
      // Get the Maven tool.
      // ** NOTE: This 'M3' Maven tool must be configured
      // **       in the global configuration.           
      //mvnHome = tool 'M3'
      mvnHome = /usr/share/maven
   }
   stage('Build') {
      // Run the maven build
      
         sh "'${mvnHome}/bin/mvn' clean deploy"
   }
   

   }
