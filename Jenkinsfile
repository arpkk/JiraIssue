pipeline {
    agent any 
    tools{nodejs "nodejs"}
    environment {
	    TEXTISSUE = "${params.TextIssue}"
    }
    stages {
        stage('Build') { 
            steps {
		echo "hace algo"
		echo "$TEXTISSUE"

		sh """
		curl --location --request POST 'https://pruebaqmetry.atlassian.net/rest/api/3/issue?textoAEnviar=Test' \
		--header 'Authorization: Basic Z2luYS5vemltaXNhQHRzb2Z0Z2xvYmFsLmNvbTpQclRkRkdiNmxvMEtLQXk5Rzd0cTI2NkM=' \
		--header 'Content-Type: application/json' \
		--header 'Cookie: atlassian.xsrf.token=5d3b4c67-268c-48e9-b2df-7d68175487ac_e9b0ba25c6a3ddeafd00fc4e74c28c189aac7608_lin' \
		--data-raw '{
		    "fields": {
			"summary": "$TEXTISSUE",
			"issuetype": {
			    "id": "10002"
			},
			"project": {
			    "key": "IR"
			},
			"description": {
			    "type": "doc",
			    "version": 1,
			    "content": [
				{
				    "type": "paragraph",
				    "content": [
					{
					    "text": "$TEXTISSUE",
					    "type": "text"
					}
				    ]
				}
			    ]
			}
		    }
		}'
		    
		    
		    
		    
		"""
	    }
        }
    }
}
