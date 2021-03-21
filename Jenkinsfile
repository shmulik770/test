#!/usr/bin/env groovy
pipeline {
     agent any

        stages {
        stage('Run Tests') {
            parallel {
                stage('parallel 1') {
                    steps {
                        sh 'pytest'
                    }
                }
                stage('parallel 2') {
                    steps {
                        echo "parallel 2"
                    }
                }
            }
        }
    }
}