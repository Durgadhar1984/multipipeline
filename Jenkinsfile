node('master') 
{
    stage('ContinuousDownload_master') 
    {
       git 'https://github.com/Durgadhar1984/multipipeline.git'
    }
    stage('ContinuousBuild_master')
    {
        sh label: '', script: 'mvn package'
    }
    
}
