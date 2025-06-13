pipeline {
    agent any
    environment {
        PYTHON_HOME = "/usr/bin/python3" 
    }
    stages {
	stage('Install Dependencies'){
	    steps {
	        sh 'pip install pandas'
	    }	
	}
        stage('Run Data_Analysis') {
            steps {
                sh 'python3 data_analysis.py' 
            }
        }
    }
}
