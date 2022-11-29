pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
            	sh "npm run changevariable"
				sh newman run json.json
            }
        }
    }
}