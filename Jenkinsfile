properties([pipelineTriggers([githubPush()])])

pipeline {
    agent { dockerfile true }
    stages {
        stages('Lancement playbook'){
            colorized: true,
            become: true,
            playbook: 'ansible-playbooks/playbook.yml'
        }
    }
}
