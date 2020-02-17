pipeline {
    agent any
    stages {
      stage('Upload to AWS'){
        steps {
            withAWS(region:'ap-south-1',credentials:'AKIA5XBPFJS53NCJJOFV') {
                s3Upload(file:'inhtmldex.txt', bucket:'jenkins-setup-1')
            }
        }
      }
    }
}
