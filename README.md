# Postman & Newman for your CICD

English version

## User Summary

Postman is a tool that allows users to simply and quickly call APIs. Its intuitive interface, the ability to save and share query collections, as well as various other features have made this tool very popular among developers. What you may not know is that Postman now has a CLI companion called Newman. Newman is an open-source command-line client for launching Postman collections. The integration of Postman collections into the CICD then became possible.

In this session, we will show you how to create a Postman collection from an Open API specification for use in a CICD process with Newman. We will cover the techniques to treat different use cases such as synchronous call, asynchronous call, workflow, etc. Finally, Newman is also a nodejs library, which opens the possibilities of extension and customization. Coming out of this conference, you will see Postman in a different way because, in addition to being an excellent tool to manually test APIs, now it allows you to reuse your already created collections in your CICD.

## For Member of Jury

Postman user since long enough, I just discovered the Newman project. In this session, I want to share this combination Postman and Newman that I find very practical. We can now easily run the same tests from our desktops in our CICD pipeline. The presentation will consist of:

Introductory slides on Postman and Newman main features. Demonstration of the creation of a collection from an OpenAPI specification (Swagger) to its integration in a Jenkins pipeline.
Demonstration of several use cases such as Synchronous, Asynchronous, and Workflow.

Here are the provisional contents of the conference in details:
- Postman Introduction
- Postman collections
- Postman environments
- Request + Runner
- Pre-request + Test
- Other features: workspace, team sharing, sandbox / mock, monitoring

- Newman Introduction
- ClI Postman
- Nodejs library (npm)

### Demonstration

Context: Test an application exposing a REST API (OpenAPI)
- Import the OpenAPI specification to Postman
- Create environments
- Authentication management
- Creation of tests
- Test the asynchronous case (use Postman echo)
- Test the implementation of test workflow
- Use the Runner on Postman
- Export the collection and the environment
- Run the runner using Newman
- Integrate Newman into the CICD (Jenkins pipeline)
- Show Newman's report
- Show how to use the Newman library in Serverless for monitoring / alerting

### Conclusion:
Positive points: People are already using Postman, so we facilitate the creation of automated tests (no need to use another language/framework like Cucumber / Karate)

Negative points: No management of integrated secrets. Limited collection sharing

## References :
- https://www.getpostman.com/downloads/
- https://github.com/postmanlabs/newman
- https://www.npmjs.com/package/newman
- https://github.com/keraton/flight-service : demo project
