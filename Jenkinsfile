pipeline {
	agent { docker { image 'python:3.7.2' } } 
	stages{
		stage("Run Python Test") {
			steps {
				sh "python tests.py"
			}
		}
	}
}