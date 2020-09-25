pipeline
{
    agent { label "kosipipelineexecutor" }
    stages
    {
        stage('Prepare')
        {
            steps
            {
                echo "${STAGE_NAME}"                                
            }
        }
        stage('Parallel Build')
        {
            parallel()
            {
                stage('Build A')
                {
                    agent { label "kosipipelineexecutor" }
                    stages
                    {
                        stage('Build')
                        {
                            steps
                            {
                                echo "${STAGE_NAME}"                                
                            }
                        }
                        stage('Test')
                        {
                            steps
                            {
                                echo "${STAGE_NAME}"                                
                            }
                        }
                    }
                }
                stage('Build B')
                {
                    agent { label "kosipipelineexecutor" }
                    stages
                    {
                        stage('Build')
                        {
                            steps
                            {
                                echo "${STAGE_NAME}"                                
                            }
                        }
                        stage('Test')
                        {
                            steps
                            {
                                echo "${STAGE_NAME}"                                
                            }
                        }
                    }
                }
                stage('Build C')
                {
                    agent { label "kosipipelineexecutor" }
                    stages
                    {
                        stage('Build')
                        {
                            steps
                            {
                                echo "${STAGE_NAME}"                                
                            }
                        }
                        stage('Test')
                        {
                            steps
                            {
                                echo "${STAGE_NAME}"                                
                            }
                        }
                    }
                }
            }
        }
        stage('Deploy')
        {
            steps
            {
                echo "${STAGE_NAME}"                                
            }
        }
    }
}
