stage 'snapshot build'
node {
    echo 'Hello from snapshot'
}

stage 'snapshot deploy'
node {
    echo 'Hello from snapshot deploy'
}

stage 'PR to master'
def userInput = input(
 id: 'userInput', message: 'Let\'s promote?', parameters: [
 [$class: 'TextParameterDefinition', defaultValue: 'uat', description: 'Environment', name: 'env'],
 [$class: 'TextParameterDefinition', defaultValue: 'uat1', description: 'Target', name: 'target']
]) 
echo ("Env: "+userInput['env'])
echo ("Target: "+userInput['target'])

node {
    echo 'Hello from snapshot'
}
