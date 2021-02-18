# The immudb Coding Challenge - Winter 2020 Edition

```
  The first immudb Coding Challenge is over and we're thrilled by the submissions! Many thanks to all participants and congratulations to the winners!
```

## Winners

- 1st place - Oscar Fernandez (https://github.com/oscarpfernandez)
- 2nd place - Antonio Navarro Perez (https://github.com/ajnavarro/immusql)


<img align="right" src="https://codenotary.io/images/immudb/mascot.png" width="160px" />To all Gophers and data modeling wizards out there: do we have a challenge for you!!
Today we announce our first #immuchallenge coding competition - Winter 2020 Edition. 

The challenge: **Design and implement a document-like data model on immudb** 

Our Open Source immudb immutable datastore builds on the traditional key-value data model guaranteeing immutability  in a quite unique manner. This simple yet generic data model provides the basis for the design of more complex and challenging immutable data models - like document-like data models.

## Instructions

A document data model is composed of identifiable elements which have properties and may be related to other elements in many different ways. For more information about document data models, we've listed some helpful [resources](#More-Resources) below.

We expect a minimal functional implementation written in Go (including unit testing) - either fully integrated into immudb or as a standalone component. The new immutable document data model needs to be built on top of the immudb immutable key-value model in order to leverage immutability properties. 

Below are the commands for getting the immudb Docker image using a Linux shell. You'll find more details about how to download and get started with immudb in our [developer jumpstart](https://docs.immudb.io/0.9.0/jumpstart.html).

1. Pull immudb Docker Image from Docker Hub:

```sh
docker pull codenotary/immudb:latest
```

2. Run immudb in a container:

```sh
docker run -it -d -p 3322:3322 -p 9497:9497 --name immudb codenotary/immudb:latest
```

In developing your solution, you'll have to make decisions that are related to:

1. **API** which stores and retrieves documents and provide proof of no tampering 
2. **Data format** which defines how objects are exchanged between final application and storage 
3. **Atomicity** at the level of document property, single, or multiple document 
4. **Concurrency** to allow concurrent read and update operations 
5. **Granularity** of evidence to prove whether a whole document or only the document property is unchanged and untampered

Please submit your solution via email to challenge@vchain.us before **February 15th, 2021, 0:00AM CST**. All code submitted at a later time, will not be included in our decision process.

## Competition Price Assignment Panel 

Our panel is comprised of Jerónimo Irázabal, immudb maintainer and project manager, Dennis Zimmer, CTO of vChain, and Michele Meloni, immudb core developer.

The two winners of the competition will be announced on this page on February 18th, 2021. We will select the best data models based on design decisions, implementation and performance as well as overall code quality. 

Feel free to also share your approach, testing, and/or anything interesting you have learned in the #immuchallenge channel in [slack](https://open-immutability.slack.com). 

## Prizes

- 1st place - **$750** (Amazon.com Gift Card)
- 2nd place - **$350** (Amazon.com Gift Card)

## Questions & Clarifications

For further questions and modifications, contact jeronimo@vchain.us. 

## More Resources

[immudb repository](https://github.com/codenotary/immudb)

[immudb website](https://codenotary.io/technologies/immudb/)

[immudb documentation](https://docs.immudb.io/)

immudb SDKs:

1. Java: [immudb4j](https://github.com/codenotary/immudb4j)
2. Golang: [immudb-go](https://docs.immudb.io/0.9.0/sdks-api.html)
3. .NET: [immudb4dotnet](https://github.com/codenotary/immudb4dotnet)
4. Python: [immudb-py](https://github.com/codenotary/immudb-py)
5. Node.js: [immudb-node](https://github.com/codenotary/immudb-node)

Document data model references:

1. https://en.wikipedia.org/wiki/Document-oriented_database
2. https://www.mongodb.com/document-databases
3. https://aws.amazon.com/nosql/document/
4. https://apple.github.io/foundationdb/data-modeling.html#documents

[Privacy Statement](https://codenotary.io/privacy-statement)
