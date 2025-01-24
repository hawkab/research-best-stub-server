# research-best-stub-server
Research on: What is the best mocking solution for services for development, debugging and integration testing of applications in Java ecosystem?

EN | [RU](README_ru.md)

# Analysis of existing solutions, comparison of characteristics

|Tool|Main Application|Ease of Use|Support for Complex Logic|Response Format|Deployment Method|Features|
|---|---|---|---|---|---|---|
|[WireMock](https://wiremock.org/)|REST и SOAP API|Medium|High|JSON, XML, other|Java application, Docker|Record and play requests, integrate with tests|
|[MockServer](https://www.mock-server.com/)|HTTP/HTTPS заглушки|Medium|High|Any|Java, standalone, Docker|Dynamic behavior change|
|[Postman Mock Server](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/)|Prototypes and quick checks|Very simple|Low|JSON|Built in Postman|Easy to configure, dynamic variables|
|[JSON Server](https://github.com/typicode/json-server)|Простые REST API|Very Simple|Low|JSON|Node.js app|Minimal effort: JSON file only|
|[Beeceptor](https://beeceptor.com/)|Quickly create stubs|Very simple|Medium|JSON|Cloud service|Convenient web interface, no local installation|
|[Mountebank](https://www.mbtest.org/)|Different protocols (HTTP, TCP, SMTP)|Medium|High|Any|Node.js, standalone|Universality, suitable for multi-protocol systems|
|[Hoverfly](https://hoverfly.io/)|High Load Systems|Medium|High|JSON|Standalone, Docker|Support for recording and replaying requests|
|[Fastify (Mock Plugin)](https://fastify.dev/)|Node.js с Fastify|Simple|Low|JSON|Node.js app|Integrates well into Fastify projects|
|[Spring Cloud Contract](https://spring.io/projects/spring-cloud-contract)|Java и Spring|Medium|High|JSON, XML, other|Spring app, Docker|Contract testing, generating stubs from contracts|



# Approximate time estimate for implementation of each tool:

|*Tool*|*Simple Scenarios*|*Complex Scenarios*|*Comments*|
|---|---|---|---|
|WireMock|1-2 hours|1-2 days|Requires DSL or JSON configuration, suitable for integration into Java projects.|
|MockServer|1-3 hours|1-2 days|A bit more complex to set up, especially for complex rules. Suitable for flexible scenarios.|
|Postman Mock Server|15-30 minutes|1-2 hours|Very easy to use GUI, no programming required.|
|JSON Server|15-30 minutes|Not applicable|Fast deployment, but limited capabilities for complex logic.|
|Beeceptor|5-15 minutes|1-2 hours|Fully cloud-based solution, minimal setup.|
|Mountebank|1-2 hours|1-3 days|Supports different protocols, requires time to study the documentation.|
|Hoverfly|1-2 hours|1-2 days|Convenient for recording and playing back requests, easy to set up.|
|Fastify (Mock Plugin)|30 minutes - 1 hour|1-2 days|A simple tool for those who already work with Fastify (Node.js).|
|Spring Cloud Contract|1-3 hours|1-2 days|Suitable for Java/Spring projects, requires knowledge of contract testing.|


# Licensing

|*Tool*|*Free*|*Paid Features*|
|---|---|---|
|WireMock|Yes (Open Source)|WireMock Cloud (cloud version): additional features, scalability.|
|MockServer|Yes (Open Source)|No paid features.|
|Postman Mock Server|Partially (Free Plan)|Free plan has a limited number of requests. Paid plans for larger requests and teamwork.|
|JSON Server|Yes (Open Source)|No paid features.|
|Beeceptor|Partially (Free Plan)|Free plan has a limited number of requests per month. Paid plans for larger volumes.|
|Mountebank|Yes (Open Source)|No paid features.|
|Hoverfly|Yes (Open Source)|No paid features.|
|Fastify (Mock Plugin)|Yes (Open Source)|No paid features.|
|Spring Cloud Contract|Yes (Open Source)|No paid features.|


# A comparative table describing the community activity and number of questions on Stack Overflow:

|*Tool*|*Community Size*|*Stack Overflow Questions*|*Additional Metrics*|
|---|---|---|---|
|WireMock|Large and active community. Over 5 million downloads per month. Has a Slack channel and a GitHub project.|[2700+​](https://stackoverflow.com/search?q=WireMock)|Extensive documentation, ready-made API templates, and a cloud version for use in teams.|
|Spring Cloud Contract|Large community|[757+](https://stackoverflow.com/search?q=Spring+Cloud+Contract)|Maintained by a community on GitHub and other channels.|
|MockServer|Smaller but more focused community with activity on GitHub and a user forum.|[990+](https://stackoverflow.com/search?q=MockServer)|Mailing list for users and active discussion on GitHub.|
|Postman Mock Server|Narrow-focused community, popular for microservices, less active than WireMock.|[220+](https://stackoverflow.com/search?q=Postman+Mock+Server)|Large user community via Postman (many use for API testing).|
|Beeceptor|Narrow-focused community|[28+](https://stackoverflow.com/search?q=Beeceptor)| |
|Mountebank|Narrow-focused community|[129+](https://stackoverflow.com/search?q=Mountebank)|Maintained by an active community on GitHub.|
|Hoverfly|Narrow-focused community|[66+](https://stackoverflow.com/search?q=Hoverfly)|Support is limited to active contributors to the project.|
|Fastify (Mock Plugin)|Highly specialized community|[8+](https://stackoverflow.com/search?q=Fastify+%28Mock+Plugin%29)|Active community of Fastify developers.|


# In conclusion

I think that Wiremock is the most suitable candidate, due to the fact that:

* has the most active community
* tight integration with Java,
* ability to work outside the Java ecosystem for universal integration with other systems
* license Apache License 2.0 (free)
* supports complex mappings, but has an average implementation time.
  
Documentation: https://wiremock.org/docs/download-and-installation/
