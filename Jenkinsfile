node {
    stage('Preparation') {
        git 'https://github.com/rkowdeed/testNG.git'
    }
    stage('install'){
        bat 'mvn clean install' // Dependency Installation stage
    }
    stage('Scan') {
        snykSecurity organisation: 'prashant.b', projectName: 'testNG', severity: 'medium', snykInstallation: 'Snyk', snykTokenId: '7ce508d2-94b3-4790-b545-089627ab64ff', targetFile: 'package.jar'
    }
    stage('Build') {
        echo "Build"
    }
    stage('Results') {
        echo "Test Result"
    }
}