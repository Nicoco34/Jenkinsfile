pipeline {
    agent any
    stages {
        stage('Build') {
    steps {
        parallel (
            "Windows" : {
                echo 'done'
            },
            "Linux" : {
                echo 'done'
            }
        )
     }
} 
        }
        stage('build2') {
            steps {
                input 'Do you approve deployment?'
                echo 'Ceci est le build1'
                build job: 'test1', parameters: [string(name: 'var', value: 'coucou build2')]
            }
        }
    }
}
