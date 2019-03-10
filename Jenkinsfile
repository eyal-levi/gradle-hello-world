node('slave1') {
    def gradleHome = tool 'gradle4'
    stages {
        stage('checkout') {
            steps {
                checkout scm
            }
        }
        stage('build') {
            steps{
                sh "${gradleHome}/gradlew build”
            }
        }
    }
}
