pipeline {
    agent any 
    tools{
	nodejs "nodejs"
    }
    stages {
        stage('Build') { 
            steps {
		echo "hace algo"
		sh " npm cache clean"
            	sh "npm run changevariable.js"
		sh "npm install -g newman"
            	echo Jira.postman_collection.json
		echo json.json
		sh "newman run json.json"
            }
        }
    }
}
