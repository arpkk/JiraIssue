pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
            	sh "npm run changevariable"
            	echo Jira.postman_collection.json
		sh "newman run json.json"
            }
        }
    }
}
