
pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                echo 'Compiling Java program...'
                bat 'javac HelloJenkins.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Executing Java program...'
                bat 'java HelloJenkins'
            }
        }
    }

    post {
        success {
            echo 'Build completed successfully!'
        }
        failure {
            echo 'Build failed. Please check the Console Output.'
        }
    }
}
