pipeline {
    agent any

    stages{
        stage('Get Git repo'){
            stage{
                steps
                {
                    git url:'https://github.com/skakella/pipeline.git',branch:'master'    
                }
            }
        }
        stage('install-git on remote'){
            steps{
                sh 'ansible-playbook agent install-git.yml' 
            }

        }
    }
}

