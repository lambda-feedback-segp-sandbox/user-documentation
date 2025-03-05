# Advanced users

Advanced users can develop their own evaluation functions.

## Evaluation functions

Evaluation functions are responsible for taking in a user's response, comparing it with a correct answer, and providing feedback to the frontend application. Living as containserized Lambda functions on the cloud, they are infinitely customisable and language-agnostic. Content authors should be able to create their own at will. However, we are aware that in a lot of cases, this grading logic will be similar, which is why a few functions have already been created.

[Evaluation functions - Quickstart Guide](evaluation_functions/quickstart.md){ .md-button .md-button--primary }

## Response areas

Response areas are components in the frontend where student users can enter a response. The response is sent to the evaluation function, which returns feedback to the response area. In the alpha version response areas are built into the software (rather than being modular) so are not straightforward to redevelop. This website catalogues the basic behaviour of response areas, to inform developers of evaluation functions.

[Response areas - overview](response_areas/overview.md){ .md-button .md-button--primary}

## AI Chatbot Agents

Chatbot agents are AI Assistants that students can chat with to ask for help or further explanations regarding the Question that they are working on. Each Agent has its own personality and approach to assisting the students.

[Chatbot Agents - Quickstart guide](chatbot_agents/quickstart.md){ .md-button .md-button--primary}

## Response Area Sandbox

The response area sandbox is a lightweight plugin for [Storybook](https://storybook.js.org/) designed for developers to build, test and interact with newly developed response areas in an isolated envrionment that closely resembles the full Lambda Feedback website. It also suppports newly developed evaluation functions to be run against these response area components. Developers can use the [template repository](https://github.com/lambda-feedback-segp-sandbox/response-area-template) with all the prerequisite setup in place to get started with the development of new response area. Click the button below to find out more!

[Response Area Sandbox - Quickstart](response_area_sandbox/sand_box.md){ .md-button .md-button--primary}

## System Architecture

- Technologies
- Deployment pipelines
- Hierarchy

## Future Features
