node {
    
    stage('Clone') {
        checkout scm
    }
    
    stage('Playbook') {
        /*sh 'ansible-playbook playbook.yml -i inventaire.ini -vvv'*/
        ansiblePlaybook become: true, credentialsId: 'ansible1', inventory: 'inventaire.ini', playbook: 'playbook.yml'
        
    }
    
    
}
