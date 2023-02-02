pipeline {
    agent { label 'ansible' }
    stages {
        stage ('git clone') {
            steps {
                git branch: "main",
                url: "https://github.com/Srikanthreddy1000/Ansible-jenkins.git" 
            }
        }
        stage ('ansible') {
            steps {
                sh "ansible -i hosts -m ping all"
            }
        }
    }
}