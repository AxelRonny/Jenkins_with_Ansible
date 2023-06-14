node {
    
    stage('Clone') {
        checkout scm
    }
    
    stage('Playbook') {
        /*sh 'ansible-playbook playbook.yml -i inventaire.ini -vvv'*/
        /*ePlaybook become: true, credentialsId: 'ansible1', inventory: 'inventaire.ini', playbook: 'playbook.yml'*/
        ansible-playbook playbook.yml -i inventaire.ini -b --become-user root --private-key /home/momo/.ssh/ansible1_key.pem -u momo
        
        
    }
    
    
}
