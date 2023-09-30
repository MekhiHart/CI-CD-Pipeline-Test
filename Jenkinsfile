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
                    sh "python3 -m pytest"
                }
            }
        }
        
        
    }
}