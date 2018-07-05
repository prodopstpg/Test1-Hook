if(env.BRANCH_NAME == 'master'){
    stage 'build master'
    node{
        def job = build job: '100%	For-master'
     }
}
else if(env.BRANCH_NAME == 'Dev'){
    stage 'build Dev'
    node{
        def job = build job: 'For-master'
    }
}
        
