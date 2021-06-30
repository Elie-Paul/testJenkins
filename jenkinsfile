pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/Elie-Paul/testJenkins"
            }
        }
        stage('build') { 
            steps {
                sh "cd testJenkins/ && javac Main.java"
            }
        }
        stage('run') { 
            steps {
                sh "cd testJenkins/ && java Main"
            }
        }
    }
}
