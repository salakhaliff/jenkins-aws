pipeline {
    agent any
    stages {
        stage('Copy') {
            steps {
                aws s3 cp s3://sala-sample-bucket/ai_5_logo_alone.png .
            }
        }
    }
}
