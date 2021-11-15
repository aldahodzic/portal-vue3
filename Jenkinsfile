pipeline {
    agent { label 'linux' }

    stages {
        stage('Build') {
            steps {
                nodejs(nodeJSInstallationName: 'Node') {
                    sh 'npm install'
                    sh 'npm run build'
                }
            }
        }

    }

}