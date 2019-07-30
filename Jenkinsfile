pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package'
		sh 'pwd'
		sh 'cp target/*.jar ../packages/' 
		sh 'cd ../packages'
		sh 'ls'
            }
        }
    }
}
