
node {

    stage('Initialize') {
        def mavenHome  = tool 'myMaven'
        env.PATH = "${mavenHome}/bin:${env.PATH}"
    }

    stage('Checkout') {
        checkout scm
    }

    stage('Test'){
        sh "mvn clean test"
    }

}
