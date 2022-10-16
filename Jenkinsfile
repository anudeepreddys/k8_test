pipeline {
    agent any

    stages {
        stage('deploy') {
            steps {
                script{
                    kubernetesDeploy configs: 'sample_app.yaml', kubeConfig: [path: ''], kubeconfigId: 'config_k8', secretName: '', ssh: [sshCredentialsId: '*', sshServer: ''], textCredentials: [certificateAuthorityData: '', clientCertificateData: '', clientKeyData: '', serverUrl: 'https://']
                }
            }
        }
    }
}
