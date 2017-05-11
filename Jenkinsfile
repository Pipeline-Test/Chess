#!groovy

node {
    checkout scm
    stage("Start") {
        sh "echo I can has sucjbjbnububyhbcess?"
        def testImg = docker.build("ugomadagu/clouldjenkins:latest");
        
       // withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: "$pipeline", usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD']]) {
       //     testImg.push();
       // }
        
    }
}
