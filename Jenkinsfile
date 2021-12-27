pipeline {
	agent none 
	stages {
		stage('Build') { 
			agent {
				docker {
					image 'python:2-alpine' 
				}
			}
			steps {
				sh 'python -m py_compile add2vals.py calc.py' 
				stash(name: 'compiled-results', includes: '*.py*') 
			}
		}
	}
}