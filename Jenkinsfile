#!groovy

node {
    checkout scm
    stage("Start") {
        sh "echo I can has sucjbjbnububyhbcess?"
        def testImg = docker.build("ugomadagu/clouldjenkins:latest");
        
        
        Docker.withRegistry("https://hub.docker.com/", "$dockercert") {
          env_img.push()
        }
        
    }
}
