pipeline {
	agent { docker { image 'python:3.10.1-alpine' } }
	stages{
		stage("Run Python Test") {
			steps {
				sh "python tests.py"
			}
		}
	}
}