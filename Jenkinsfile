pipeline {
    agent any

    parameters {
        string(defaultValue: "DEV", description: 'What environment?', name: 'Environment')
        choice(choices: ['DEV', 'QA', 'QA2'], description: 'select environment', name: 'options')
        string(name: 'company_parameter', defaultValue: '', description: 'The company the pipeline runs in')
        string(name: 'test1', defaultValue: '', description: 'The company the pipeline runs in')
    }
    


    stages {
        stage("foo") {
            steps {
                  sh "echo ${params.options}"
                  sh "echo ${params.company_parameter}"
                  sh "echo ${params.test1}"
            }
        }
    }
}
