# lambda-test
A Lambda function is the core of the serverless architecture on AWS.

When you define and implement a lambda function you publish it on your AWS account and you pay it per execution.

```
exports.findClosestEnemy = (event, context, callback) => {
  callback(null,"OK"); /* JOB DONE, END EXECUTION*/
}
```

# parameters

## event: input JSON object (e.g. {"field1":"value1"})

## callback: the callback function that you need to call to end execution of the lambda

## context: a collection of variables and methods that describe the execution environment (e.g. the function name), this is not useful for this test's purpose.
