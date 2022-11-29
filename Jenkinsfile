pipeline {
    agent any 
    tools{nodejs "nodejs"}
    stages {
	    stage("Prep for per-dir Jenkinsfile") {
            checkout(scm)
            sh 'git clean -fdx'
          }
        stage('Build') { 
            steps {
		echo "hace algo"
            	sh 'npm run changevariable.js'
		sh 'npm install -g newman'
            	echo Jira.postman_collection.json
		echo json.json
		sh 'newman run json.json'
            }
        }
    }
}
