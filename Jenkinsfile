pipeline {
    // Run the pipeline on any available agent
    agent any

    // Define the parameters for the pipeline
    parameters {
        string(
            name: 'STAGE_NAME_1',
            defaultValue: 'First Stage',
            description: 'The name for the first stage.'
        )
        string(
            name: 'STAGE_NAME_2',
            defaultValue: 'Second Stage',
            description: 'The name for the second stage.'
        )
    }

    // Define the stages
    stages {
        stage('Echo First Parameter') {
            steps {
                echo "The name of the first stage is as : ${params.STAGE_NAME_1}"
            }
        }
        stage('Echo Second Parameter') {
            steps {
                echo "The name of the second stage is: ${params.STAGE_NAME_2}"
            }
        }
    }
}
