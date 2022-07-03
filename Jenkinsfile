node {
  stage('SCM') {
    // git clone
    git 'https://github.com/sabeer-hussain/JUnit4-and-Maven-Example.git'
  }

  stage('build the packages') {
    //mvn clean package
    sh 'mvn clean package'
  }

   stage ('archival') {
     // archiving artifacts
     archiveArtifacts 'target/*.jar'
   }

}