#!/usr/bin/env groovy

node {
    stage('checkout') {
        checkout scm
    }
    docker.image('openjdk:8').inside('-u root -e MAVEN_OPTS="-Duser.home=./"') {
    stage('check java') {
        sh "java -version"
    }

}
