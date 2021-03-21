#!/usr/bin/env groovy
pipeline {
     agent any

    stages {
        stage("Test") {
 			parallel {
                stage('parallel 1') {
                      test: {
                        sh 'pytest'
                      },
                      echo: {
                        echo "echo parallel 1"
                      }
                  }
                stage('parallel 2') {
                      test: {
                        sh 'pytest'
                      },
                      echo: {
                        echo "echo parallel 2"
                      }
                  }
                )
			}
        }
    }
}