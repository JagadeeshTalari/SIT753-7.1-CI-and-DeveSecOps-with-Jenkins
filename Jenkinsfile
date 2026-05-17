pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compile and package the source code into a deployable artifact.'
                echo 'Tool: Maven - a build automation tool that manages dependencies and compiles Java code.'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Run unit tests to verify individual components work correctly.'
                echo 'Task: Run integration tests to verify components work together.'
                echo 'Tools: JUnit for unit tests, Selenium for integration tests.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analyse the code for quality issues, code smells, and standards compliance.'
                echo 'Tool: SonarQube - a static code analysis tool integrated with Jenkins.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scan the code and dependencies for known vulnerabilities (CVEs).'
                echo 'Tool: OWASP Dependency-Check - identifies vulnerable libraries in the project.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploy the packaged application to a staging server for pre-production testing.'
                echo 'Tool: AWS CLI - used to deploy to an AWS EC2 staging instance.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Run integration tests against the staging environment to simulate production behavior.'
                echo 'Tool: Postman/Newman - API testing tool for end-to-end integration tests.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploy the tested and approved application to the live production server.'
                echo 'Tool: AWS CLI - used to deploy to an AWS EC2 production instance.'
            }
        }
    }
}