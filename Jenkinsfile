pipeline {
    agent none
    stages {
        stage('Run Tests') {
            parallel {
                stage('run shell script') {
                    agent {
                        label "windows"
                    }
                    steps {
                        sh './hello.sh'
                    }
                }
                stage('test stage') {
                    agent {
                        label "linux"
                    }
                    steps {
                        sh 'touch newfile.sh'
                    }
                   
                }
            }
        }
    }
}
