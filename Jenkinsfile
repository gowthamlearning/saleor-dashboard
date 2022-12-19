pipeline {
    agent {label 'docker'}
    stages {
        stage ('src') {
            steps{
                git url:"https://github.com/gowthamlearning/saleor-dashboard.git",
                    branch:"main"
            }
        }
        stage('build image') {
            sh """ docker image build -t gowthi1404/saleor-dashboard:dev-19122022 .
               docker image push gowthi1404/saleor-dashboard:dev-19122022 """
        }
    }
}