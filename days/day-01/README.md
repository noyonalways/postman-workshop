<img src='https://i.ibb.co/K9bDjSv/Day-1-Mastering-API-Testing-and-Environment-Management-on-Postman.jpg' width='100%' alt='banner-image' style='border-radius: 10px' />

# Day- 01: Mastering API Testing Environment Management

## ToTo Company (API Providers)

### API Types:

- Public
- Private / Internal
- Partner

**Public:**

Access by anyone with API key

**Private / Internal:**

Used within the same org. Access is restricted (OAuth, OpenID connect) communication between different services

**Partner:**

Access by different organizations. Access is restricted. Agreements between creator and consumer.

### Focus on the Following Problems

---

- **Documentation Deficiency:** Their API lack proper documentation. For instance details on how their partners should call API endpoints from different clients, the necessary payload, headers required for sending requests etc. are missing.
- **Validation and Testing Gaps:** There are no solutions in place to validate or test their API responses.
- **Collaboration Challenges:** There is problem with collaboration and easily sharing API’s with across the development team.
- **Environment Mix-up:** They cannot easily manage their APIs in different environment (e.g. development, testing, production)
- **Performance Analysis Dilemma:** They lack an easy solution to analyze and identify performance issues, errors, or any unexpected behavior in their APIs hampering improvements.
- **Frontend-Backend Coordination Issues:** They regularly observe that their frontend teams sometimes wait for the backend to complete APIs., causing delays in completing projects on time.
- **Unclear authorization process:** Toto company uses OAuth2 and OpenID connect to secure their APIs. However, their backend team often receives questions from the frontend team, such as “Frontend team is unable to authorize and obtain a token from the authorization server.” This is common for the frontend team because the backend team cannot demonstrate simple steps to work with their Auth server.
- **Data-Driven Testing Hurdles:** They want to perform Data-Driven testing.
- **Automated Testing Goals:** They also aim to automated their API testing process, generating reports automatically.
- **API Data Flows:** Their backend team desire a system where they can directly manipulate APIs and observe the data flowing between them without creating a new application. This helps them creates a mind map of their API functionality.

### After one week completing research their RND team introduce with a HERO called **[POSTMAN](https://www.postman.com/downloads/)**

## What is Postman?

Postman is a popular collaboration platform for API development. It provides a
user-friendly interface that allows developers to design, test, document, and share APIs
effortlessly. Some key features of Postman include:

- **API Testing:** Postman allows developers to create and execute automated tests
  for APIs, making it easier to ensure the reliability and functionality of APIs.
- **API Documentation:** Developers can generate comprehensive documentation for
  APIs within Postman, making it easier for other developers to understand how to
  use them.
- **Mock Servers:** Postman allows developers to create mock servers for APIs,
  enabling them to simulate API behavior without actually implementing the
  backend logic, which is useful for testing and development purposes.
- **API Monitoring:** Postman offers monitoring capabilities to track the performance
  and uptime of APIs, helping developers identify and resolve issues quickly.
- **API Collections:** Postman allows users to organize APIs into collections, making
  it easier to manage and share sets of related APIs with team members or the
  broader community

With Postman, developers can seamlessly interact with a wide range of API types,
including REST, GraphQL, gRPC, WebSockets, and more.

### In short:

**Postman** is a popular API Client that allows you to make requests to APIs. Test API endpoints and automate API testing. It provides a use-friendly interface for constructing and sending HTTP requests, as well as for inspecting the response. Postman also offers features for collaboration, documenting APIs and Monitoring API etc.

### What is an API Client?

An **API Client** is a set of tools and protocols that operate form an application on a computer. They help you to bypass some operations when developing a web application rather than reinventing the wheel every time. Using a client API is a great way to speed up the development process.

# Let’s Explore Postman

## Postman Collections

Now let’s talk about the postman collections. Postman collections are an essential feature of the Postman platform, serving as a convenient way to organize, manage, and share APIs and requests.

**Here are some key features of Postman collections:**

- **Organization:** Collections enable you to organize API requests logically, making
  it easier to manage and navigate through your APIs
- **Sharing:** You can share collections with team members or the broader
  community, facilitating collaboration and knowledge sharing.
- **Documentation:** Collections can include documentation, making it simple to
  provide detailed information about each API request, including parameters,
  headers, and response examples.
- **Testing:** Collections allow you to include test scripts, enabling automated testing
  of APIs as part of your workflow.
- **Environments:** Collections support the use of environments, allowing you to
  define variables that can be used across multiple requests within the collection.
  This is particularly useful for managing different environments such as
  development, staging, and production.

SO, collection is a grouping or container for a set of related API requests. It allows you to organize, structure, and logically manage your API requests. Collections can include multiple requests, scripts, and even folders to help you streamline and categorize your API development and testing workflows

### In Short:

In Postman a collection is a grouping or container for a set of related API requests. It allows you to organize, structure, and manage your API requests in a logical manner. Collections can include multiple requests, scripts and even folders to help you streamline categorize your API development and testing workflows.

## Postman Variables

When discussing Postman collections, it's essential to delve into Postman variables. Without a grasp of Postman variables, you can't fully leverage the benefits offered by the Postman platform. These variables are crucial components that enhance flexibility, reusability, and efficiency in managing API requests, scripts, and environments. They empower developers to streamline workflows, simplify maintenance, and ensure dynamic data handling across different testing and development scenarios. In essence, understanding and effectively utilizing Postman variables are fundamental steps toward maximizing the potential of the Postman tool set.

### In Postman there are 5 types of variables available:

1. Global Variables
2. Collection Variables
3. Environment Variables
4. Data Variables
5. Local Variables

**Here is the details overview:**

- **Global variables** enable you to access data between collections, requests, and
  test scripts. Global variables are available throughout a workspace. Global
  variables are a helpful tool for sharing variables across the workspace.
- **Collection variables** are available throughout the requests in a collection.
  Collection variables are useful for keeping variables private within a collection of
  APIs and don't want to share variables outside the collection.
- **Environment variables** enable you to scope your work to different
  environments, for example, Development and testing. One environment can be
  active at a time.
- **Data Variables** in your data come from external CSV and JSON files. You use
  these sets of data when running collections with Newman or the Collection
  Runner. These variables have current values that only last during the request or
  collection runs.
- **Local variables** are temporary variables that are accessed in your request
  scripts. Local variable values are scoped to a single request or collection run and
  are no longer available when the run is complete. Local variables are suitable if
  you need a value to override all other variable scopes but don't want the value to
  persist once execution has ended.

## Postman Variables Diagram

<img src='https://i.ibb.co/c2yvgRN/postman-variables-diagram.png' alt='postman-variables-diagram' width='100%'>

## Postman Scripts Diagram

<img src='https://i.ibb.co/NjMpcyk/image.png' alt='postman-script-diagram' width='100%'>
