if(env.BRANCH_NAME == 'master'){
    stage("Upload"){
        sh ('Mtest.sh')
    }
}
else if(env.BRANCH_NAME == 'Dev'){
    stage("Deploy"){
    //dir('/var/lib/jenkins/Ankit_script'){
        sh ('Test.sh')
        echo "from Dev"
    }
}
        
