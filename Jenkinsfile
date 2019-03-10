node('slave1') {
    stages {
        stage('checkout') {
            checkout scm
        }
        stage('build') {
            def gradleHome = tool 'gradle4'
            sh "${gradleHome}/bin/gradle build”
        }
    }
}
