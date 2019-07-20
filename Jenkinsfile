#! groovy

node(){
  stage('prepareWorksapce'){
        echo "====Hello World===="
  }
  
  stage('checkout'){
    checkout([$class: 'GitSCM',
              branches: [[name: '*/master']],
              doGenerateSubmoduleConfigurations: false,
              extensions: [], submoduleCfg: [],
              userRemoteConfigs: [[url: 'https://github.com/devdoc24/test.git']]])
  }

}
