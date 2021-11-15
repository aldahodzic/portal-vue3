pipeline {
    agent { label 'linux' }

    stages {
        stage('Build') {
            steps {
                nodejs(nodeJSInstallationName: 'Node') {
                    sh 'rm -rf node_modules package-lock.json'
                    sh 'npm cache clear --force'
                    sh 'npm install'
                    sh 'npm run build'
                }
            }
        }

    }

}