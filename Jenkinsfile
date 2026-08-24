pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'python -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'python -m pytest test_app.py -v'
            }
        }

        stage('Run Application') {
            steps {
                bat 'python app.py'
            }
        }
    }

    post {
        success {
            echo '✅ Build and tests completed successfully!'
        }

        failure {
            echo '❌ Pipeline failed. Check the logs.'
        }

        always {
            echo 'Pipeline execution completed.'
        }
    }
}
