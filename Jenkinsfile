pipeline {
         agent any
         stages {
                 stage('stage 0 : Checkout from root Github repo') {
                 steps {
                     echo 'Checkout successfully'
                     git 'https://github.com/chethancg/helloworld.git'
                 }
                 stage('stage 1 : Build') {
                 steps {
                     echo 'Build successfully'
                          bat label: '', script: '''javac HelloWorld.java 
                                                    java HelloWorld'''
                       }
                 }
                 stage('stage 2 : Test') {
                 steps {
                     echo 'Tested successfully'
                 }
                 }
                 stage('stage 3 : Deploy') {
                 steps {
                     echo 'Deployed successfully'
                 }
                 }
        }
  }
