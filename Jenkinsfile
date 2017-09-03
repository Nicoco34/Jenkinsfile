pipeline {
    agent any
    stages {
        stage('Example') {
            input 'Do you approve deployment?'
            steps {
                echo 'Hello World'
                build job: 'test1', parameters: [string(name: 'var', value: 'coucou')]
            }
        }
    }
}
