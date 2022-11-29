pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                let json=Jira.postman_collection.json;
				let keys=JSON.parse(json);
				keys.text=${textIssue} 
				sh newman run json.json
            }
        }
    }
}