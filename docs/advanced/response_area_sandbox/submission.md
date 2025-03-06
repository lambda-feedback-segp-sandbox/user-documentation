# Submission of Response Areas to Lambda Feedback

Once the development of the response area in the sandbox is complete it is then ready to be sent to the Lambda Feedback team for review and deployment.

### Generating the File for Submission

1. To generate the file for submission run the command: 

    ```
    $ yarn build
    ```

    This will generate the file(s) in the `dist` directory of the template repository. Within this directory there will exist a file called `web-components.js`. This is the generated file for the response area that has been developed in the sandbox. 

2. Once this is complete extract this file and rename it based on the name that you have given it from the `RESPONSE_TYPE` constant in the `index.ts` file from withtin the `components` directory. This constant was what was set to define the unique name for the response area. 

3. After this then submit that `js` file to the lambda feedback team for review. 

4. (Lambda Feedback team only) Once a submission is received it can be analysed and tested within the full application stack. Once the component has satisfied all testing it can then be deployed to the application by uploading it into the AWS bucket which contains all the response areas that the application uses.

