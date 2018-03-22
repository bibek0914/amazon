pipeline {
agenet any
 stages {
  stage('compile stage') {
   steps {
    withmaven(maven: MAVEN_HOME) {
     sh mvn 'clean compile'
    }
   }
  }
   stage('testing stage') {
   steps {
    withmaven(maven: MAVEN_HOME) {
     sh mvn 'test'
    }
   }
  }
   
  stage('deploy stage') {
   steps {
    withmaven(maven: MAVEN_HOME) {
     sh mvn 'deploy'
    }
   }
  }
  
  
 }
 
}
