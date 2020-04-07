node('master') 
{
    stage('ContinuousDownload_loan') 
    {
       git 'https://github.com/Durgadhar1984/multipipeline.git'
    }
    stage('ContinuousBuild_loan')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_loan')
    {
        sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war ubuntu@172.31.92.242:/var/lib/tomcat8/webapps/testapp.war'
    }
    
}
