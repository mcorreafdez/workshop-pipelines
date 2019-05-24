#!groovy

pipeline {
    agent {
        // how the pipeline will be built
      docker {
        image 'adoptopenjdk/openjdk11:jdk-11.0.3_7'
        args '--network ci --mount type=volume,source=ci-maven-home,target=/root/.m2'
        }
    }

//    environment {
        // properties or environment variables, new or derived
//    }

    stages {
        stage('Compile') {
            steps {
               echo "-=- compiling project -=-"
               sh "./mvnw clean compile"
            }
        }
    }

//    post {
//        // post-process activities, e.g. cleanup or publish
//    }
}
