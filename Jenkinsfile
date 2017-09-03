pipeline {
    agent any
        stage("Parallel") 
            steps {
                parallel (
                    "firstTask" : {
                        echo 'Ceci est le build1'
                    },
                    "secondTask" : {
                        echo 'Ceci est le build1'
                    }
                )   
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
