node {
    
    stage('Clone') {
        checkout scm
    }
    
    stage('Playbook') {
        /*sh 'ansible-playbook playbook.yml -i inventaire.ini -vvv'*/
        ansiblePlaybook become: true, credentialsId: 'ansible1_privatekey', inventory: 'inventaire.ini', playbook: 'playbook.yml'
        /*sh 'ansible-playbook playbook.yml -i inventaire.ini --become-user root --private-key /var/lib/jenkins/workspace/.ssh/ansible1_key.pem -u momo'*/
        
        
    }
    
    
}
