pipeline {
    agent any
    stages {
      stage('Upload to AWS'){
        steps {
            withAWS(region:'ap-south-1',credentials:'aws-static') {
                s3Upload(file:'index.html', bucket:'jenkins-setup-1')
            }
        }
      }
    }
}
