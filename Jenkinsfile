node {
    label 'Dev'

    stage('Clone sources') {
        git url: 'https://github.com/manjunaths77/CelcomJava.git'
    }

    stage('Ant build') {
        sh 'ant -f build.xml'
    }
}
