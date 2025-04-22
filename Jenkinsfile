pipeline {
    agent any // or specify a specific agent

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/nurlailasari/selenium-jenkins-test.git' // Replace with your Git repository URL
            }
        }
        
        stage('Run Selenium Tests') {
            steps {
                // Add commands to run your Selenium tests (e.g., using Maven)
                sh 'mvn test' // Replace with your build command
            }
        }

        stage('Publish Test Results') {
            steps {
                // Configure test result reporting (e.g., using the JUnit plugin)
                junit '**/TEST-*.xml' // Example JUnit report path
            }
        }
    }
}
