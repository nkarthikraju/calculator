pipeline {
	agent any
	stages {
		stage('IfMaster') {
			when {
				branch 'master'
			}	
			steps {
				echo "hello This is master branch"
			}
		}
		stage('Develop') {
			when {
				branch 'NewBranch'
			}	
			steps {
				//checkout scm 
                git branch: 'NewBranch', url: 'https://github.com/nkarthikraju/calculator.git'
                echo "\n\n\n Assume this is version 1 modified in file checkoutscmex.txt file, \n next 3 versions will do on checkoutscmex.txt file and test checkout scm syntax\n"
			}}}}
			