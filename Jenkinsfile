pipeline{
    agent any 
    environment {
        DIRECTORY_PATH = "/Users/sparshdeepsingh/Documents/Jenkins/first.Jenkinsfile"
        TESTING_ENVIRONMENT = "FIRST PIPLELINE"
        PRODUCTION_ENVIRONMENT = "SPARSHDEEP SINGH"
         
    }
    stages{
        stage('Build'){
            steps{
                echo"Fetch the source code from the directory path specified by the environment variable"
                echo"Compile the code and generate any necessary artefacts"
            }
        }
        stage('Test'){
            steps{
                echo"Unit tests"
                echo"Integration tests"
            }
        }
        stage('Code Quality Check'){
            steps{
                echo"Check the quality of the code"
            }
        }
        stage('Deploy'){
            steps{
                echo"Deploy the application to a testing environment specified by the environment variable"
            }
        }
        stage('Approval'){
            steps{
                sleep 10
            }
        }
        stage('Deploy to Production'){
            steps{
                echo"Deploying the code to $PRODUCTION_ENVIRONMENT"
            }
        }
          
    }
}