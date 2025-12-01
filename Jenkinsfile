pipeline {
agent none
stages {

stage("build & SonarQube Scanner") {
agent any
steps {
withSonarQubeEnv('SonarScanner') {
sh 'mvn clean package sonar:sonar'
}
}
}
}
}
