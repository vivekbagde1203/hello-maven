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
                git branch: 'master', url: 'https://github.com/vivekbagde1203/hello-maven.git'
            }
        }
        stage("Build"){
            steps {
                mavenBuild()
            }
        }
    }
}
