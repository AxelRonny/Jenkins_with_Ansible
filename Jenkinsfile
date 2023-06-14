node {
    
    stage('Clone') {
        checkout scm
    }
    
    stage('Playbook') {
        /*sh 'ansible-playbook playbook.yml -i inventaire.ini -vvv'*/
        ansiblePlaybook become: true, credentialsId: 'ansible1' 'ansible2', inventory: 'inventaire.ini', playbook: 'playbook.yml'
         /*sh 'ansible-playbook playbook.yml -i inventaire.ini --become-user root --private-key .ssh/ansible1_key.pem -u momo'*/
        /*ansiblePlaybook credentialsId: 'ansible1', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'inventaire.ini', playbook: 'playbook.yml'*/
        
        
    }
    
    
}
