pipeline {
    agent any
    stage 'deployment'
input 'Do you approve deployment?'
node{
                    echo 'Hello World'
                build job: 'test1', parameters: [string(name: 'var', value: 'coucou')]
}
