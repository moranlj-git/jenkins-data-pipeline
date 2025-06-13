pipeline {
    agent any
    stages {
	stage('Install Dependencies'){
	    steps {
	        sh 'python3 -m venv venv'
	        sh 'source venv/bin/activate'
	        sh 'pip install pandas'
	    }	
	}
        stage('Build') {
            steps {
                script {
                    // Choisissez la commande en fonction de votre script
		    sh 'source venv/bin/activate'
                    sh 'python data_analysis.py' // Exécuter le script Python
                }
            }
        }
    }
}
