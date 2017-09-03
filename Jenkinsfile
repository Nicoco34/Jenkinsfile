pipeline {
    agent any
    stages {
        stage('build1') {
            steps {
                    input 'Do you approve deployment?'
                    echo 'Ceci est le build1'
                    build job: 'test1', parameters: [string(name: 'var', value: 'coucou build1')]
            }
            parallel(firstTask: {
  stage 'B1'
  echo 'Ceci est le build1'
}, secondTask: {
  stage 'B2'
  echo 'Ceci est le build1'
})
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
