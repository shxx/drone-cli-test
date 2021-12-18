pipeline {
    agent any

    parameters {
        // 选择分支发布
        gitParameter branchFilter: 'origin/(.*)', defaultValue: 'dev', name: 'BRANCH', type: 'PT_BRANCH', listSize: '25'
    }

    stages {
        stage('Git pull') {
            steps {
                // 下载代码
                git credentialsId: '336cca7e3f067722196eb3dd6ae1f361a911c73b', branch: "${params.BRANCH}", url: 'https://github.com/shxx/drone-cli-test.git'
            }
        }
    }

}

