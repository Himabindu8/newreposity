
    dsl script{
        job('DSL-Tutorial-1-Test') {
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
