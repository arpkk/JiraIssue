pipeline {
    agent any 
    tools{nodejs "nodejs"}
    stages {
        stage('Build') { 
            steps {
		echo "hace algo"
		echo "$TEXTISSUE"
		sh 'npm install -g curl'
            }
        }
    }
}
