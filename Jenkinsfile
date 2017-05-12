#!groovy

node {
    checkout scm
    stage("Start") {
        sh "echo I can has sucjbjbnububyhbcess?"
        def testImg = docker.build("ugomadagu/clouldjenkins:Ugo");
        //testImg.push()
        
        docker.withRegistry("", "dockercert") {
          testImg.push()
        }
        
    }
}
