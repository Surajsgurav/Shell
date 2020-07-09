pipeline {
    agent any
    stages {
      stage('run shell script') {

            steps {
                   sh './hello.sh'
                  }
              }
        stage('test stage') {

            steps {
                   sh 'touch newfile.sh'
                  }
              }
             }
           }

