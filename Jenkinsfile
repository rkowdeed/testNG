node {
    stage('Preparation') {
        git 'https://github.com/rkowdeed/testNG.git'
    }
    stage('install'){
        bat 'mvn clean install' // Dependency Installation stage
    }
    stage('Scan') {
        echo "See Synk site"
    }
    stage('Build') {
        echo "Build"
    }
    stage('Results') {
        echo "Test Result"
    }
}