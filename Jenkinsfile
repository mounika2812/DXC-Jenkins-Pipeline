pipeline{
    agent any
    
    stages{
        stage('Test'){
            steps{
                bat 'echo This is good command'
            }
        }
    }
    
    post{
        always{
            bat 'echo I will always get executed'
        }
        success{
            bat 'echo I will only get executed when the job is success'
        }
        failure{
            bat 'echo I will only get executed when the job is failed'
        }
        unstable{
            bat 'echo I will only get executed when the job is unstable'
        }
        
    }
}
