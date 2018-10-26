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
				checkout scm 
                //git branch: 'NewBranch', url: 'https://github.com/nkarthikraju/calculator.git'
                echo "Adding the checkout scm and not changing 
			}}}}
			