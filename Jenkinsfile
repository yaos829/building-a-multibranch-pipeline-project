pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
		sh 'pwd'
            }
        }
    }
}
