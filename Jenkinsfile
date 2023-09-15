pipeline {
    //agent { docker { image 'node:13.8' } }
    agent any
	stages {
        stage('Build') {
            steps {
              //  sh 'node --version'
                echo "Build"
            }
        }
        stage('Test') {
            steps {
                echo "Test"
            }
        }
        stage('Integration Test') {
            steps {
                echo "Integration Test"
            }
        }
    }
    post {
        always {
            echo 'I\'m Awesome. I Run always'
        }
        success {
            echo 'I run when you are successful'
        }
        failure {
            echo 'I run when you fail'
        }
    }
}
