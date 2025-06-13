pipeline {
    agent any
    environment {
        PATH = "${env.PATH}:/usr/bin/python3" 
    }
    stages {
	stage('Install Dependencies'){
	    steps {
	        sh 'source venv/bin/activate'
	        sh 'pip install pandas'
	    }	
	}
        stage('Build') {
            steps {
                script {
                    // Choisissez la commande en fonction de votre script
		    sh 'source venv/bin/activate'
                    sh 'python3 data_analysis.py' // Exécuter le script Python
                }
            }
        }
    }
}
