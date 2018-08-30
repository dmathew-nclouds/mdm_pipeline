

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
        stage('Run DR Post Setup') {
            parallel {
                stage('MDM1 Post Setup') {
                    
                    steps {
                        echo "MDM1 Chef Post  Setup "
                    }
                    
                }
                stage('MDM2 Post Setup') {
                    
                    steps {
                        echo "MDM2 Chef Post  Setup "
                    }
                    
                }
            }
        }
        stage('DNS Update') {
            steps {
                echo 'DNS update for DR region'
            }
        }
    }
}


