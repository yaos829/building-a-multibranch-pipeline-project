pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
        }
	stage('get clone'){
            //check CODE
	    steps {
		echo 'Checkout==========.........' 
		checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/yaos829/building-a-multibranch-pipeline-project.git']]])
            } 
    	}
    }
}
