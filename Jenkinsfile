#! groovy

node(){
        
        triggers {
        pollSCM '* * * * *'
    }
        
  stage('prepareWorksapce'){
        echo "====Hello World===="
  }
  
  stage('checkout'){
    checkout([$class: 'GitSCM',
              poll: true,
              branches: [[name: '*/master']],
              doGenerateSubmoduleConfigurations: false,
              extensions: [], submoduleCfg: [],
              userRemoteConfigs: [[url: 'https://github.com/devdoc24/test.git']]])
  }
  

}
