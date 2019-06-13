node {

    stage('checkout') {
        git branch: 'master', credentialsId: env.GIT_SIGN, url: 'http://gitlab.top.mw/devops/dockerfile.git'
    }

    stage('compile') {
        sh "cd ${env.soft} && make"
    }

}