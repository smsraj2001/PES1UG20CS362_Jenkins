pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -C main'
                echo 'Build Stage is Successful !!!'
            }
        }
        stage('Test') {
            steps {
                sh '/var/jenkins_home/workspace/PES1UG20CS362-1/main/hello_exec'
                echo 'Test Stage is Successful !!!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployed Task Sucessfully !!!'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed !!!'
            }
    }
}
