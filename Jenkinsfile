pipeline {
    agent { label 'master1111' }

    stages {
        stage('Pull Code') {
            steps {
                git branch: 'main', url: 'https://github.com/1llusionary/jenkins_go_test.git'
            }
        }
        stage('Run') {
            steps {
                sh 'go build hello.go'
                sh './hello'
            }
        }
    }
}
