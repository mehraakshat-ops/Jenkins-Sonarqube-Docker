pipeline {
    agent any
    stages {
        stage('SSH Connection') {
            steps {
                sshCommand remote: [
                    name: 'Docker Server',
                    host: '3.110.166.99',
                    user: 'ubuntu',
                    credentialsId: 'ubuntu-ssh-key',
                    port: 22
                ], command: 'echo "Jenkins SSH Working!"'
            }
        }
    }
}
