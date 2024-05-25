pipeline {
    agent any
    environment {
        AWS_ACCESS_KEY_ID     = credentials('accesskey')
        AWS_SECRET_ACCESS_KEY = credentials('secretkey')
    }
    stages {
        stage('Installing Grafana') {
            steps {
                script {
                    ansiblePlaybook(
                        playbook: 'test.yml',
                        inventory: 'inventory',
                        credentialsId: 'grafana.pem'
                    )
                }
            }
        }
    }
}
