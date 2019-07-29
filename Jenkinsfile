pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
		sh 'sshpass -p 'js20181220' scp target/my-app-1.0-SNAPSHOT.jar root@192.168.1.23:/data/packages'
            }
        }
    }
}
