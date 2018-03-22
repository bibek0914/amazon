pipeline {
agenet any
 stages {
  stage('compile stage') {
   steps {
    withmaven(maven: mvn_3.5.0) {
     sh mvn 'clean compile'
    }
   }
  }
   stage('testing stage') {
   steps {
    withmaven(maven: mvn_3.5.0) {
     sh mvn 'test'
    }
   }
  }
   stage('compile stage') {
   steps {
    withmaven(maven: mvn_3.5.0) {
     sh mvn 'clean compile'
    }
   }
  }
  stage('deploy stage') {
   steps {
    withmaven(maven: mvn_3.5.0) {
     sh mvn 'deploy'
    }
   }
  }
  
  
 }
 
}
