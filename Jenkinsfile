pipeline {
    agent any
    stages {
	// clone the repository
        stage('Clone Repository') {
            steps {
		// Replace with your repo URL
              git branch: 'main'  , url: 'https://github.com/hitu-1995/jenkinsPipelineRepo.git'  
            }
        }
	// Deploy the index.html file
        stage('Deploy HTML file') {
            steps {
		sh '''
		# Deploy index.html file to the web server directory
		cp index.html /var/www/html/
		cp contact.html /var/www/html/
		cp about.html /var/www/html/
		cp style.css /var/www/html/
		'''
            }
        }
    }
}
