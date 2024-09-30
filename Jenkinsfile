pipeline {
    agent any 

    stages {
        stage('Récupérer le code source') {
            steps {
                echo 'Récupération du code depuis le dépôt Git...'
                // Ceci est géré automatiquement si vous utilisez le SCM configuré
            }
        }

        stage('Afficher la date système') {
            steps {
                script {
                    def date = new Date()
                    echo "La date et l'heure système actuelle : ${date.format('yyyy-MM-dd HH:mm:ss')}"
                }
            }
        }
    }

    post {
        success {
            echo 'Le pipeline s\'est terminé avec succès!'
        }
        failure {
            echo 'Le pipeline a échoué.'
        }
    }
}
