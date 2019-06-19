# lambda-test
A Lambda function is the core of the serverless architecture on AWS.

When you define and implement a lambda function you publish it on your AWS account and you pay it per execution.

```
exports.functionHandler = (event, context, callback) => {
  callback(null,"OK"); /* JOB DONE, END EXECUTION*/
}
```

# parameters

```
event: input JSON object (e.g. {"field1":"value1"})
```
```
callback: the callback function that you need to call to end execution of the lambda
```
```
context: a collection of variables and methods that describe the execution environment (e.g. the function name), this is not useful for this test's purpose.
```


# test setup

You should already have [NodeJS](https://nodejs.org/en/download/) and npm installed

It is required that you use at least NodeJS v8 (async/await syntax supported)

### install lambda local

Get [lambda-local](https://www.npmjs.com/package/lambda-local)  in order to test the execution of your code, we expect that your code runs with preset inputs as well as with general inputs.

You can find lambda local usage instructions on lambda local npm page.
