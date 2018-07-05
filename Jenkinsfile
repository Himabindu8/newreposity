freeStyleJob(String DSLTEST, Closure closure = null) 
def myJob = freeStyleJob('SimpleJob')
myJob.with {
    description 'A Simple Job'
    dsl script{
        job('DSL-Tutorial-0-Test') {
        scm {
        git('https://github.com//Himabindu8//newreposity.git')
        }
    triggers {
        scm('H/15 * * * *')
    }
    steps {
        maven('-e clean test')
    }
    }
}
