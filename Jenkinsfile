pipeline {
agent none
stages {

stage("build & SonarQube Scanner") {
agent any
steps {
withSonarQubeEnv('sonarqube-25.11.0.114957') {
sh 'mvn clean verify sonar:sonar'
}
}
}
}
}
