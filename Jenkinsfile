pipeline {
    agent any
    parameters {
        string defaultValue: 'master', 
        description: 'choose the branch to build and deploy', 
        name: 'branchName', 
        trim: false
    }

    stages {
        stage ('SCM Checkout'){
            steps {
                git branch: "${params['branchName']}",
                url: "https://github.com/pranatgit/jenkins-pranat-javahomes"
            }
        }
    }
}
