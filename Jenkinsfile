@Library("vivek-shared-library") _

pipeline {
    agent any
    stages {
        stage("Greet") {
            steps {
                hello("Vivek Bagde")
            }
        }
        stage("Checkout"){
            steps {
                checkout scm
            }
        }
        stage("Build"){
            steps {
                mavenBuild()
            }
        }
    }
}
