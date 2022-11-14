pipeline{
    agent any
    tools {
        maven 'my-mvn'
    }
    stages{
        stage('build'){
            steps{
                echo "building the java app "
                sh 'mvn clean package build ' 
                //added some comments to test webhook 
            }
        }
        stage('deploy'){
            steps{
                echo 'for now this is a test job that i just created'
            }
        }
    }
}