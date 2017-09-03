pipeline {
    input 'Do you approve deployment?'
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                build job: 'test1', parameters: [string(name: 'var', value: 'coucou')]
            }
        }
    }
}
