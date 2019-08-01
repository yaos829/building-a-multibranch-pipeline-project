pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
		sh 'git log'
		sh 'git log origin/master'
                sh 'mvn -B -DskipTests clean package'
		sh 'pwd'
		sh 'rm -rf ../packages/*.jar'
		sh 'cp target/*.jar ../packages/'
		sh 'rm -rf *'
		sh 'ls -l'
            }
        }
    }
}
