pipeline {
	agent any
	stages{
		stage("Run Python Test") {
			agent { 
				docker { 
					image 'python:3.10.1-alpine' 
				} 
			}
			steps {
				sh "python tests.py"
			}
		}
	}
}