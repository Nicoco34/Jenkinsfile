pipeline {
    agent any
        stage('Parallel') 
            steps {
                parallel (
                    'firstTask' : {
                        echo 'Ceci est le build1'
                    },
                    'secondTask' : {
                        echo 'Ceci est le build1'
                    }
                )   
    }
