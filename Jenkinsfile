pipeline {
    agent any

    stages {
        stage('CloudFormation Provision') {
            steps {

                sh "aws cloudformation create-stack --stack-name myteststack12345 --template-body file://parent-stack.yaml --parameters ParameterKey=Environment,ParameterValue=Test"
            }
        }
    }
}
