pipeline 
{
    agent any

    stages 
    {
        stage('build')
        {
            steps
            {
                echo 'build App'
            }
        }
        stage('Test')
        {
            steps
            {
                echo 'Test App'
            }
        }
            stage('Deploy')
            {
                steps
                {
                    echo 'Deploy App'
                }
            }
        }
        post
        {
            always
            {
                emailext body: 'pipeline pass', subject: 'pipeline status', to: 'jnandini225@gmail.com'
            }
        }
    }

