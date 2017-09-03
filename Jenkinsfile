pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                input 'Do you approve deployment?'
                echo 'Hello World'
                build job: 'test1', parameters: [string(name: 'var', value: 'coucou')]
            }
        }
    }
}
