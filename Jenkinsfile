 pipeline {
        agent any
        stages {
            stage('Test') {
                steps {
                    echo 'Hello World from master ...'
                }
            }
            stage ('Bootstrap') {
               sh "echo GIT_BRANCH_LOCAL=\\\"$GIT_BRANCH\\\" | sed -e 's|origin/||g' | tee version.properties"
          }

           stage('Checkout') {
              load('version.properties')
              checkout([$class: 'GitSCM', branches: [[name: '**']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'LocalBranch', localBranch: "${GIT_BRANCH_LOCAL}"]], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/webofmars/grails-website.git']]])
          }
        }
    }
