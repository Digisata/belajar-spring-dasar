pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }
    stages {
        stage("Hello") {
            steps {
                echo("Hello pipeline")
            }
        }
    }
    post {
        always {
            echo "Will always say hello"
        }
        success {
            echo "Uraa, success"
        }
        failure {
            echo "Oh noo, failure"
        }
        cleanup {
            echo "Clean cleaaan"
        }
    }
}
