pipeline{
    agent{
        label "amz-linux"
    }
    stages{
        stage("Check ansible version"){
            steps{
                echo "========executing A========"
                sh 'ansible --version'
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}