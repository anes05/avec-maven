pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M2_HOME"
    }

    stages {
        stage('GIT') {
            steps {
                git branch: 'main',
                url: 'https://github.com/anes05/avec-maven.git'
            }
            
        }
        stage('Maven'){
            steps{
                sh "mvn -version"
            }
        }
    }
}