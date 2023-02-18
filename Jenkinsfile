pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS825.cpp'
                sh 'g++ -o PES1UG20CS825 PES1UG20CS825.cpp'
                echo 'Build Stage Completed Successfully'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS82'
                echo 'Test Stage Successfully Executed '
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployment was Successfull'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
