pipeline {
    agent {
        node {
            label 'Dev'
        }
    }

    environment {
        PATH = "$HOME/apache-ant-1.10.10/bin:$PATH"
    }
    stages {
        stage('Environment') {
            steps {
                    sh "hostname"
            }
        }
            }   
            steps {
            //    ws('/home/jenkins/thiru') {
                    // Run Maven on a Unix agent.
                    sh "echo $PATH"
                    sh "id"
                    sh 'ant -f build.xml'
            //    }
            }   
        }
    }
}
