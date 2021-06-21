pipeline {
    agent {
        node {
            label 'Dev'
            customWorkspace "/home/manjus/thiru/Master"
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
        stage('checkout') {
            steps {
            // Get some code from a GitHub repositor
            //    ws('/home/jenkins/thiru') {
                   git 'https://github.com/manjunaths77/CelcomJava.git'
            //    }
            }
        }
        stage('Build') {
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
