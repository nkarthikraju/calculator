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
                bat '''
                @echo off
                set /p txt=What do you want it to say? ; 
               rem echo %txt% >C:/Users/namburuk/Desktop/temp/ex.txt"
                echo %hi% >>C:/Users/namburuk/Desktop/temp/ex.txt"
                '''
			}
		}
	}
}
