if(env.BRANCH_NAME == 'master'){
    stage("Upload"){
        sh '"echo "from master"'
    }
}
else if(env.BRANCH_NAME == 'Dev'){
    stage("Deploy"){
        sh 'echo "Dev"'
    }
}
        
