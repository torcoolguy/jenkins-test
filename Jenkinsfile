pipeline {
    agent any
    stages {
        stage('Testing') {
            steps {
                echo 'Kubernetes test...'
                kubernetesDeploy(
                    kubeconfigId: 'kubeconfig',
                    configs: 'kube-test.yml'
                )
            }
        }
    }
}