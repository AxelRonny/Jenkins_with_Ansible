node {
    
    stage('Clone') {
        checkout scm
    }
    
    stage('Playbook') {
        sh 'ansible-playbook playbook.yml -i inventaire.ini -vvv'
        
    }
    
    
}
