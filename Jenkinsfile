pipeline {
  agent any
  options {
    skipStagesAfterUnstable()
  }
  stages {
    stage('Deploy to Docker') {
      steps {
        script {
            kubernetesDeploy configs: 'sample_app.yaml', kubeConfig: [path: ''], kubeconfigId: '12c5b643-4c43-49f6-8f24-6da6786a7cc5', secretName: '', ssh: [sshCredentialsId: '*', sshServer: ''], textCredentials: [certificateAuthorityData: '', clientCertificateData: '', clientKeyData: '', serverUrl: 'https://']
       }
      }
    }
  }
}
