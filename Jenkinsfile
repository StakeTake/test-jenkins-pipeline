pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Клонируем репозиторий
                checkout scm
            }
        }
        stage('Install Dependencies') {
            steps {
                // Устанавливаем зависимости
                sh 'pip3 install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                // Запускаем тесты
                sh 'pytest'
            }
        }
    }
}
