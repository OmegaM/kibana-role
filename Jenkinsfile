pipeline{
    agent any
    stages{
        stage('SCM'){
            steps{
                git credentialsId: 'github', url: 'git@github.com:OmegaM/kibana-role.git'
            }
        }
        
        stage('Test'){
            steps{
                sh 'molecule test'
            }
        }
        
    }
}
