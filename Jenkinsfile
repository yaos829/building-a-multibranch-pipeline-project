pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package'
		sh 'sshpass -p js20181220 scp target/*.jar root@192.168.1.23:/data/packages' 
            }
        }
    }
}
