pipeline {
	agent {
		label "slave-1"
		customWorkspace "/mnt/pipeline"
	}
	stages {
		stage("Stage 1") {
			steps {
				script {
					sh "sudo service httpd start"
					sh "sudo cp -r index.html /var/www/html/"
					sh "sudo chmod -R 777 /var/www/html/index.html"
				}
			}
		}
	}
}
