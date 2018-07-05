 pipeline {
        agent any
        stages {
            stage('Test') {
                steps {
                    echo 'Hello World from master ...'
                    echo "${GIT_LOCAL_BRANCH}"
                }
            }   
        }
    }
