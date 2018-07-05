freeStyleJob('JENKINS_JOB'){ 
   jdk('java  8')
          scm {
        github('jenkinsci/job-dsl-plugin','master')
        }
    triggers {
        scm('H/15 * * * *')
    }
    steps {
        maven('-e clean test')
       }
}


