# Request Response Cycle, APIs, and Postman Lab

You will be working with a free API of your choice for this lab.

## Getting Started

1. Choose an API with no auth and no CORS from the following list. It _should not_ be one that you've already seen or worked on in class.
   - [Public APIs](https://github.com/public-apis/public-apis)
1. Choose an API not covered in your readings, class, or other assignments. The API should be new to you.
1. Write your answers in this README.md file. Do not delete the questions. Write your answers after the `>`. If you need to write more than one paragraph, add more `>`.
1. Take the time to read back the work, and edit what you've written so that your answers are clear and anyone reading it can easily understand what you've written.

## Instructions

Do your best to answer the questions with specific details. Writing about code clearly and thoroughly is a critical skill to practice.

- Which one did you choose? Provide the name and base URL.

> Cat Facts- https://cat-fact.herokuapp.com

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> Retrieve and query facts regarding cat. API provides information like text, type, created, and updated date. someone might want to add and view personal list of fact recipients, send a cat fact via text message every day, and submit their own interesting facts


- What is the URL of the documentation?

> https://alexwohlbruck.github.io/cat-facts/docs/

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> https://cat-fact.herokuapp.com/facts

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
[
    {
        "status": {
            "verified": true,
            "sentCount": 1
        },
        "_id": "58e008780aac31001185ed05",
        "user": "58e007480aac31001185ecef",
        "text": "Owning a cat can reduce the risk of stroke and heart attack by a third.",
        "__v": 0,
        "source": "user",
        "updatedAt": "2020-08-23T20:20:01.611Z",
        "type": "cat",
        "createdAt": "2018-03-29T20:20:03.844Z",
        "deleted": false,
        "used": false
    },
    {
        "status": {
            "verified": true,
            "sentCount": 1
        },
        "_id": "58e009390aac31001185ed10",
        "user": "58e007480aac31001185ecef",
        "text": "Most cats are lactose intolerant, and milk can cause painful stomach cramps and diarrhea. It's best to forego the milk and just give your cat the standard: clean, cool drinking water.",
        "__v": 0,
        "source": "user",
        "updatedAt": "2020-08-23T20:20:01.611Z",
        "type": "cat",
        "createdAt": "2018-03-04T21:20:02.979Z",
        "deleted": false,
        "used": false
    },
    {
        "status": {
            "verified": true,
            "sentCount": 1
        },
        "_id": "588e746706ac2b00110e59ff",
        "user": "588e6e8806ac2b00110e59c3",
        "text": "Domestic cats spend about 70 percent of the day sleeping and 15 percent of the day grooming.",
        "__v": 0,
        "source": "user",
        "updatedAt": "2020-08-26T20:20:02.359Z",
        "type": "cat",
        "createdAt": "2018-01-14T21:20:02.750Z",
        "deleted": false,
        "used": true
    },
    {
        "status": {
            "verified": true,
            "sentCount": 1
        },
        "_id": "58e008ad0aac31001185ed0c",
        "user": "58e007480aac31001185ecef",
        "text": "The frequency of a domestic cat's purr is the same at which muscles and bones repair themselves.",
        "__v": 0,
        "source": "user",
        "updatedAt": "2020-08-24T20:20:01.867Z",
        "type": "cat",
        "createdAt": "2018-03-15T20:20:03.281Z",
        "deleted": false,
        "used": true
    },
    {
        "status": {
            "verified": true,
            "sentCount": 1
        },
        "_id": "58e007cc0aac31001185ecf5",
        "user": "58e007480aac31001185ecef",
        "text": "Cats are the most popular pet in the United States: There are 88 million pet cats and 74 million dogs.",
        "__v": 0,
        "source": "user",
        "updatedAt": "2020-08-23T20:20:01.611Z",
        "type": "cat",
        "createdAt": "2018-03-01T21:20:02.713Z",
        "deleted": false,
        "used": false
    }
]


```

- What status code did you get back from your request? Why did you receive this status code?

> Status code: 200. This status code indicates that the request was successful. It means that the server processed the request and returned the requested data.

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`:application/json; charset=utf-8

> `Content-Length`:1863


- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The response includes a random cat fact. This fact mentions how many toes cats have on their front and back paws.

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that ...
>Create a web page that displays a cat fact for users.
>Develop an application that allows users to share cat facts on social media platforms.


### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The API documentation provides clear explanations on how to use the API and which parameters to use.

- What did you find challenging about the documentation? Cite specific examples.

> I found that examples of API usage were lacking in the documentation. More details could be provided on how to construct complex requests.

- Did the quality of the documentation impact your decision to use it?

> Yes, the quality of the documentation played a significant role in my decision to use the API. Clear and comprehensive documentation makes it easier to understand how to use the API effectively.

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> No, the quality of the documentation for the Cat Facts API influenced my decision to use it, and I didn't feel the need to switch to another API.






### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is a fundamental concept in web development that describes the process of communication between a client and a server. It begins when a client sends a request to the server, specifying what it wants to retrieve or do. The server then processes the request, performs any necessary operations, and sends back a response to the client. This response contains the requested data or indicates the outcome of the operation. The cycle continues as the client may subsequently send additional requests based on the received response.

- In your own words, describe what an API is.

> An API, or Application Programming Interface, is a set of rules, protocols, and tools that allows different software applications to communicate with each other. It defines the methods and data formats that applications can use to request and exchange information. APIs enable developers to access the functionality of other software systems or services without needing to understand their internal workings. They serve as intermediaries that facilitate seamless integration between different software components, enabling the development of complex applications.



- In your own words, describe the purpose of Postman.

> Postman is an application that simplifies the process of testing, documenting, and managing APIs. It provides an intuitive graphical user interface (GUI) that allows developers to create, send, and analyze HTTP requests and responses. With Postman, developers can easily build and organize collections of API requests, set up automated tests to verify API functionality, and generate detailed documentation for APIs. Postman streamlines the development workflow by providing a centralized platform for API testing and collaboration, helping developers to debug and troubleshoot API integrations efficiently.






