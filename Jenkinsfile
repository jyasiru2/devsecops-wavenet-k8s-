pipeline {
  agent any

  stages {
      stage('Build Artifact') {
            steps {
              sh "cd devsecops-wavenet-k8s-"
              sh "mvn clean package -DskipTests=true"
              archive 'target/*.jar' //so that they can be downloaded later
            }
        }   
    }
}
