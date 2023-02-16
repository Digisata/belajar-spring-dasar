pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }
    stages {
        stage("Build") {
            steps {
                echo("Hello Build")
            }
        }
        stage("Test") {
            steps {
                echo("Hello Test")
                sh("error")
            }
        }
        stage("Deploy") {
            steps {
                echo("Hello Deploy")
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
