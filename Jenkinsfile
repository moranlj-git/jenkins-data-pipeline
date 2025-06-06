pipeline {
    agent any
    environment {
        PYTHON_HOME = '/usr/bin/python3' 
        PATH = "${env.PATH}:${JAVA_HOME}/bin:/usr/bin" 
    }
    stages {
        stage('Build') {
            steps {
                script {
                    // Choisissez la commande en fonction de votre script
                    sh 'pip install pandas' // Installer les dépendances
                    sh 'python data_analysis.py' // Exécuter le script Python
                }
            }
        }
    }
}
