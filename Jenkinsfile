pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
		echo "hace algo"
	        sh "npm init"
		sh "npm run build"
            	sh 'npm run changevariable.js'
		sh 'npm install -g newman'
            	echo Jira.postman_collection.json
		echo json.json
		sh 'newman run json.json'
            }
        }
    }
}
