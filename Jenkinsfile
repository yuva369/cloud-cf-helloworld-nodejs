@Library('piper-lib-os') _
node() {
    stages {
        stage('Pre-Checkout') {
            steps {
                sh "git config http.sslVerify false"
            }
        }
        stage('prepare') {
            checkout scm
            setupCommonPipelineEnvironment script:this
        }
    }
}
