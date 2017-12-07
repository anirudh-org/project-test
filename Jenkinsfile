properties([
           [$class: 'GithubProjectProperty',
          displayName: '',
          projectUrlStr: 'https://github.com/anirudh-org/project-test.git'],
          pipelineTriggers([
          upstream(
           threshold: 'SUCCESS',
            upstreamProjects: 'https://github.com/anirudh-org/poject-compile.git'    )])
   ])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
     stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
