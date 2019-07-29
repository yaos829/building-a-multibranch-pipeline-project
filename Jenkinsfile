pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
		sh 'pwd'
		sh 'cd /var/lib/jenkins'
		sh 'pwd'
		sh 'cd /data/packages'
		sh 'pwd'
            }
        }
    }
}
