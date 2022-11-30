pipeline {
    agent any 
    tools{nodejs "nodejs"}
    stages {
        stage('Build') { 
            steps {
		echo "hace algo"
		echo "${params.TextIssue}"
		sh 'npm install -g curl'
	    }
        }
    }
}
