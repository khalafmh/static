pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region: 'us-east-1', credentials: 'AKIAV3KD2YFWSMOVHAPL') {
                    s3Upload(file: 'index.html', bucket: 'mahdialkhalaf-udacity-static', path: '/')
                }
            }
        }
    }
}