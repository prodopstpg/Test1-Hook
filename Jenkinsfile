if(env.BRANCH_NAME == 'master'){
    stage("Upload"){
        sh ('Mtest.sh')
        echo "branch: ${env.BRANCH_NAME}"
    }
}
else if(env.BRANCH_NAME == 'Dev'){
    stage("Deploy"){
    //dir('/var/lib/jenkins/Ankit_script'){
        sh ('Test.sh')
        echo "branch: ${env.BRANCH_NAME}"
    }
}
        
