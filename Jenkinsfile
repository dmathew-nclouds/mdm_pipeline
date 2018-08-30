

pipeline {
    agent none
    stages {
        stage('Run DR Infra Setup') {
            parallel {
                stage('MDM1 Infra Setup') {
                    
                    steps {
                        echo "MDM1 Infrastructure Terraform Setup "
                    }
                    
                }
                stage('MDM2 Infra Setup') {
                    
                    steps {
                        echo "MDM2 Infrastructure Terraform Setup "
                    }
                    
                }
            }
        }
    }
}


