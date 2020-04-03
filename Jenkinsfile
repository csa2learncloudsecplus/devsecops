#!groovypipeline{
  agentanyenvironment{
    AWS_REGION='eu-west-1'AWS_ENV=csa2''AWS_DOM=learncloudsecplus.net''
  }stages{
    stage('Build'){
      steps{
        sh'npm i'
      }
    }stage('Unit Test'){
      steps{
        sh'npm test'
      }
    }stage('Dev (Deploy)'){
      QADEVSECOPSServerlessLabPartTwoversion0.5Page13environment{
        AWS_STAGE='dev'
      }steps{
        sh'serverless deploy -s dev'
      }
    }
  }
}
