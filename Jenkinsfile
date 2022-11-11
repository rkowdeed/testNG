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
    stage('Deploy') {
        echo "${project.basedir}/target/${project.build.finalName}.jar"
    }
}