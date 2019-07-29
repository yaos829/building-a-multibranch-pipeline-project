pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
		sh 'pwd'
		sh 'scp target/my-app-1.0-SNAPSHOT.jar root@192.168.1.23:/data/packages'
		sh 'sshpass -p 'js20181220' scp target/my-app-1.0-SNAPSHOT.jar root@192.168.1.23:/data/packages'
            }
        }
    }
}
