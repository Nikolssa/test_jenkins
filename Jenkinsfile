def workspace;
node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '5049348c-7cc3-4c16-aa40-42f942813ea4', url: 'git@github.com:Nikolssa/test_jenkins.git']]])
        workspace =pwd()
    }
    stage('Static Code Analysis')
    {
        echo "Static Code Analysis"
        println("Hello From Groovy");
        for (def i = 0; i <= 10; i += 2) {
            println("Value is " + i);
        }
        def dog = "SHARIK"
        println(dog);
        dog = 10;
        println(dog);
    }
    stage('Build')
    {
        echo "Build the code"
    }
    stage('Unit Testing')
    {
        echo "Unit Testing"
    }
    stage('Delivery')
    {
        echo "Deliver the Code"
    }
}
