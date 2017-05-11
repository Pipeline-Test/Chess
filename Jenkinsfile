#!groovy

node {
    checkout scm
    stage("Start") {
        sh "echo I can has sucjbjbnububyhbcess?"
        def testImg = docker.build("ugomadagu/clouldjenkins:latest");
        
        withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: "name", usernameVariable: 'ugomadagu', passwordVariable: '8c316738d4f38d18ac99259ddb6dd5c533ea7b5d']]) {
            testImg.push();
        }
        
    }
}
