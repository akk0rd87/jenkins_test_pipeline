pipeline {
    agent any
    stages {
        stage('Build') {
            agent {
                dockerfile {
                    filename 'androidDocker.build'
                    label 'androidDocker-label'
                }
            }
            steps {
                sh 'gradle --version'
            }
        }
    }
}
