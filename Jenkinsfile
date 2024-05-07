pipeline {
	agent {
		label {
			label "slave-1"
			customWorkspace "/mnt/pipeline"
		}
	}
	stage {
		stage ("stage-1"){
		steps {		
			sh "sudo service httpd start"
			sh "sudo cp -r index.html /var/www/html/"
			sh "sudo chmod -R 777 /var/www/html/index.html
		}	
		}
	}
}
