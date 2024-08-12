pipeline {
    agent any
    stages {
        stage('Setup') {
            steps {
                // Install Node.js and dependencies
                sh 'npm install'
                sh 'npx playwright install --with-deps'
            }
        }
        stage('Run Playwright Tests') {
            steps {
                // Run Playwright tests
                sh 'npx playwright test'
            }
        }
        // Add more stages as needed (e.g., reporting, deployment)
    }
}
