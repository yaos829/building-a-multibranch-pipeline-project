pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /root/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package'
		sh 'sshpass -p js20181220 scp target/*.jar root@192.168.1.23:/data/packages' 
            }
        }
    }
}
