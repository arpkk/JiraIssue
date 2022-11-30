pipeline {
    agent any 
    tools{nodejs "nodejs"}
    environment {
	    TEXTISSUE = "${params.TEXTISSUE}"
    }
    stages {
        stage('Build') { 
            steps {
		echo "hace algo"
		echo $TEXTISSUE
		sh 'npm install -g curl'
	    }
        }
    }
}
