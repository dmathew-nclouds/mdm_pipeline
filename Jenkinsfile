

pipeline {
    agent none
    stages {
        stage('Run Tests') {
            parallel {
                stage('MDM1 Infra Setup') {
                    
                    steps {
                        echo "MDM1 Infrastructure Terraform Setup "
                    }
                    
                }
                stage('MDM1 2nfra Setup') {
                    
                    steps {
                        echo "MDM2 Infrastructure Terraform Setup "
                    }
                    
                }
            }
        }
    }
}


