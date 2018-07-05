if(env.BRANCH_NAME == 'master'){
    stage("Upload"){
        sh 'sh /var/lib/jenkins/Ankit_script/Test.sh'
    }
}
else if(env.BRANCH_NAME == 'Dev'){
    stage("Deploy"){
        sh 'sh /var/lib/jenkins/Ankit_script/Mtest.sh'
    }
}
        
