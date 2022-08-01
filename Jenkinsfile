pipeline{
    agent{
        label "amz-linux"
    }
    stages{
        stage("Check ansible version"){
            steps{
                echo "========executing A========"
                sh 'ansible --version'
                sh 'ansible-playbook -i inventory playbook.yml'
            }
        }
    }
}