pipeline{
    agent any
    stages{
        
        stage("Compile"){
            steps{
                script {
                    sh "python3 ops.py"
                }
            }
        }
        
        stage("Unit Test"){
            steps{
                script{
                    sh "coverage run -m pytest"
                }
            }
        }

        stage("Coverage Test"){
            steps{
                step{
                    sh "coverage report -m"
                }
            }
        }
        
        
    }
}