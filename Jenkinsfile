pipeline {
	agent none
	stages{
		stage("Run Python Test") {
			agent { docker { image 'python:3.7.2' } } 
			steps {
				sh "python tests.py"
			}
		}
	}
}