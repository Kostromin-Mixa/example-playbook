pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/Kostromin-Mixa/example-playbook.git'

                // Run ansible on a Unix agent.
                sh "ansible-playbook /var/lib/jenkins/workspace/Declarative/site.yml -i /var/lib/jenkins/workspace/Declarative/inventory/prod.yml"
               }
          }
     }       
}