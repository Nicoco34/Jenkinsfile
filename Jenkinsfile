pipeline {
    agent any
    stages {
        input 'Do you approve deployment?'
        stage('Example') {
            steps {
                echo 'Hello World'
                build job: 'test1', parameters: [string(name: 'var', value: 'coucou')]
            }
        }
    }
}
