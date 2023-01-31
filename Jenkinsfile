pipeline {
    agent { label 'ansible' }
    stages {
        stage ('git clone') {
            steps {
                url: "https://github.com/Srikanthreddy1000/Ansible-jenkins.git",
                git branch: "main"
            }
        }
        stage ('ansible') {
            steps {
                sh "ansible-playbook -i hosts playbook.yml"
            }
        }
    }
}