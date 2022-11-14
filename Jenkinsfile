pipeline{
    agent any
    tools {
        maven 'my-mvn'
    }
    stages{
        stage('build'){
            steps{
                echo "building the java app "
                sh 'mvn clean package' 
            }
        }
    }
}