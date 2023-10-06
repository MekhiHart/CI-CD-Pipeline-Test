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
                    sh "python3-coverage run -m pytest test_ops.py"
                }
            }
        }

        stage("Coverage Test"){
            steps{
                script{
                    sh "python3-coverage report -m"
                }
            }
        }
        
        
    }
}