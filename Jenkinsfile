

pipeline {
    agent none
    stages {
        stage('Run DR Infrastructure Setup') {
            parallel {
                stage('MDM1 Infrastructure Setup') {
                    
                    steps {
                        echo "MDM1 Infrastructure Terraform Setup "
                    }
                    
                }
                stage('MDM1 Infrastructure Setup') {
                    
                    steps {
                        echo "MDM2 Infrastructure Terraform Setup "
                    }
                    
                }
            }
        }
    }
}


