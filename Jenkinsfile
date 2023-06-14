node {
    
    stage('Clone') {
        checkout scm
    }
    
    stage('Playbook') {
        sh 'sudo ansible-playbook playbook.yml -i inventaire.ini -vvv'
        
    }
    
    
}
