pipeline {
    agent {
        docker {
            image 'python:3.11'
            args "-v ${env.WORKSPACE}:/app -w /app"
        }
    }

    parameters {
        string(name: 'NAME', defaultValue: 'World', description: 'Who to greet')
    }

    stages {
        stage('Greet') {
            steps {
                echo "Hello, ${params.NAME}!"
            }
        }
        stage('Python v') {
            steps {
                sh "py --version"
            }
        }
    }
}
