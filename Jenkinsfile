node {
  stage('SCM') {
    // git clone
    git 'https://github.com/sabeer-hussain/JUnit4-and-Maven-Example.git'
  }

  stage('build the packages') {
    //mvn package
    sh 'mvn package'
  }

   stage ('archival') {
     // archiving artifacts
     archive 'target/*.jar'
   }

}