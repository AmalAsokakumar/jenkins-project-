node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def mvn = tool 'my-mvn';
    withSonarQubeEnv() {
      sh "${mvn}/bin/mvn clean verify sonar:sonar -Dsonar.projectKey=jenkins"
    }
  }
}





// pipeline{
//     agent any
//     tools {
//         maven 'my-mvn'
//     }
//     stages{
//         stage('build'){
//             steps{
//                 echo "building the java app "
//                 sh 'mvn clean package' 
//                 //added some comments to test webhook 
//             }
//         }
//     }
// }