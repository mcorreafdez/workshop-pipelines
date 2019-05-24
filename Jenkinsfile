#!groovy

pipeline {
    agent {
        // how the pipeline will be built
      docker { image 'python:3.5.1' }      
    }

//    environment {
        // properties or environment variables, new or derived
//    }

    stages {
        stage('hello-stage') {
            steps {
                // steps for stage 1 come here
               sh "echo 'Hello'"
            }
        }
    }

//    post {
//        // post-process activities, e.g. cleanup or publish
//    }
}
