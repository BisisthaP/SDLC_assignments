pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Cloning the repo...'
                // Jenkins clones it automatically; no command needed
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Script') {
            steps {
                echo 'Running app.py...'
                sh 'python app.py'
            }
        }

        stage('Post-build') {
            steps {
                echo 'CI/CD run completed!'
            }
        }
    }
}