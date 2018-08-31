

pipeline {
    agent none
    stages {
        stage('DR Infrastructure Setup') {
            parallel {
                stage('MDM1 Infrastructure Setup') {
                    
                    steps {
                        sleep 5
                        echo "MDM1 Infrastructure Terraform Setup "
                    }
                    
                }
                stage('MDM2 Infrastructure Setup') {
                    
                    steps {
                        sleep 5
                        echo "MDM2 Infrastructure Terraform Setup "
                    }
                    
                }
            }
        }
        stage('Run DR Post Setup') {
            parallel {
                stage('MDM1 Post Setup') {
                    
                    steps {
                        sleep 5
                        echo "MDM1 Chef Post  Setup "
                    }
                    
                }
                stage('MDM2 Post Setup') {
                    
                    steps {
                        sleep 5
                        echo "MDM2 Chef Post  Setup "
                    }
                    
                }
            }
        }
        stage('DNS Update') {
            steps {
                sleep 5
                echo 'DNS update for DR region'
            }
        }
        stage('Configure Aviatrix VPN') {
            steps {
                sleep 5
                echo 'Configure Aviatrix VPN'
            }
        }

        stage('Generate Aviatrix  Client Configs') {
            steps {
                input "Generate Aviatrix  Client Configs Completed ?"
            }
        }


    }
}


