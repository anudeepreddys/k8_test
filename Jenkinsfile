pipeline {
    agent any

    stages {
        stage('deploy') {
            steps {
                script{
                    kubernetesDeploy configs: 'sample_app.yaml', kubeConfig: [path: ''], kubeconfigId: 'k8s', secretName: '', ssh: [sshCredentialsId: '*', sshServer: ''], textCredentials: [certificateAuthorityData: '', clientCertificateData: '', clientKeyData: '', serverUrl: 'https://']
                }
            }
        }
    }
}
