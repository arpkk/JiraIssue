pipeline {
    agent any 
    tools{nodejs "nodejs"}
    stages {
        stage('Build') { 
            steps {
		echo "hace algo"
		echo "$TextIssue"
		sh 'npm install -g curl'
            }
        }
    }
}
