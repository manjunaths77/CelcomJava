node {
    label 'Dev'

    stage('Clone sources') {
        git url: 'https://github.com/manjunaths77/CelcomJava.git'
    }

    stage('Ant build') {
        when {
            branch "Dev"
        }
        steps {
            sh 'ant -f build.xml'
        }
    }
}
