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

        // stage('package code')
        // {
        //     steps
        //     {
        //         withAnt(installation: 'ANT_Home', jdk: 'JDK_home') 
        //         {
        //             sh 'ant clean package -DskipTests'
        //         }        
        //     }
        // }
    }
}
