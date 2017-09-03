pipeline {
    agent any
parallel firstBranch: {
    stage ('Starting Test') 
    {
        build job: 'test1', parameters: [string(name: 'var', value: 'coucou')]
    }
}, secondBranch: {
    stage ('Starting Test2') 
    {
        build job: 'test1', parameters: [string(name: 'var', value: 'coucou')]
    }
}
