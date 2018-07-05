if(env.BRANCH_NAME == 'origin/master'){
    stage ('build master'){
        build job: 'For-master'
     }
}
else if(env.BRANCH_NAME == 'origin/Dev'){
    stage ('build Dev'){
        build job: 'For-master'
    }
}
        
