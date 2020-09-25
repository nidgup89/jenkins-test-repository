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
                stage('Build A for Windows')
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
                        stage('Deploy')
                        {
                            steps
                            {
                                echo "${STAGE_NAME}"
                            }
                        }
                    }
                }
                stage('Build B for Linux')
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
                        stage('Deploy')
                        {
                            steps
                            {
                                echo "${STAGE_NAME}"
                            }
                        }
                    }
                }
                stage('Build C for Appl-Mac')
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
                        stage('Deploy')
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
        stage('Promote')
        {
            steps
            {
                echo "${STAGE_NAME}"                                
            }
        }
    }
}
