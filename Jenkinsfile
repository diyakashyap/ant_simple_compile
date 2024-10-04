pipeline
{
    agent any
    stages
    {
        stage('compile code')
        {
            steps
            {
                withAnt(installation: 'ANT_Home', jdk: 'JDK_home') 
                {
                    sh 'ant compile'
                }        
            }
        }

        stage('package the code')
        {
            steps
            {
                withAnt(installation: 'ANT_Home', jdk: 'JDK_home') 
                {
                    sh 'ant package -DskipTests'
                }        
            }
        }
    }
}