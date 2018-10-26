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
				echo "hello This is NewBranch branch changes in new branch"
			}
		}
	}
}
