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

// The below one is for the PES1UG20CS362.cpp file :
// pipeline {
//     agent any
    
//     stages {
//         stage('Build') {
//             steps {
//                 sh 'g++ -o PES1UG20CS362-1 PES1UG20CS362.cpp'
//                 echo 'Build Stage is Successful !!!'
//             }
//         }
//         stage('Test') {
//             steps {
//                 sh './PES1UG20CS362-1'
//                 echo 'Test Stage is Successful !!!'
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 echo 'Deployed Task Sucessfully !!!'                
//             }
//         }
//     }
    
//     post {
//         failure {
//             echo 'Pipeline failed !!!'
//         }
//     }
// }
