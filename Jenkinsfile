pipeline {
    agent any

    parameters {
        string(name: 'NAME', defaultValue: 'World', description: 'Who to greet')
    }

    stages {
        stage('Greet') {
            steps {
                echo "Hello, ${params.NAME}!"
            }
        }
    }
}
