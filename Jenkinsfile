import jenkins.*
import hudson.*
import hudson.model.*
import groovy.json.JsonOutput


node{
stages{
 
               stage('Clone')
                 {
                 checkout scm
                  }
              stage('Build')
                  {
                     bat 'mvn -s $MAVEN_SETTINGS -B clean deploy cobertura:cobertura javadoc:javadoc'
                     steps {
                             maven('-e clean test')
                                 script {
                                         job('MYFIRST JOB') {
                                            scm {
                                           git('https://github.com/Himabindu8/newreposity.git')
                                                }
                                  triggers {
                                  scm('H/10 * * * *')
                                          }
                                                         }
                                         }
                                        job('MYSECOND JOB') {
                                         scm {
                                         git('https://github.com/Himabindu8/newreposity.git')
                                              }
                                        triggers {
                                       scm('H/10 * * * *')
                                                 }
                                                }
                                           }
                                      job('MYTHIRD JOB') {
                                           scm {
                                        git('https://github.com/Himabindu8/newreposity.git')
                                                }
                                        triggers {
                                               scm('H/10 * * * *')
                                                }
                                             }
                                          }  
                                     job('MYFOURTH JOB') {
                                              scm {
                                             git('https://github.com/Himabindu8/newreposity.git')
                                                 }
                                                 triggers {
                                                 scm('H/10 * * * *')
                                                        }
                                                      }
                                               } 
                                     }
 
      }
   }
