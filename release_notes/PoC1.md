# Filecoin Secondary Retrieval Market: PoC1

## New In This Release
This release includes the initial version of the following components:

* [Retrieval Gateway](https://github.com/ConsenSys/fc-retrieval-gateway): A service that runs as a single Docker container to facilitate Piece CID offers discovery.
* [Retrieval Provider](https://github.com/ConsenSys/fc-retrieval-provider): A services that runs as a single Docker container to faciliate the publishing of Piece CID offers. This service will integrate with or be associated with Filecoin storage miners.
* [Retrival Gateway Admn](https://github.com/ConsenSys/fc-retrieval-gateway-admin): A Golang library that can be integrated with an application to allow the Retreival Gateway to be administered.
* [Retrival Provider Admn](https://github.com/ConsenSys/fc-retrieval-provider-admin): A Golang library that can be integrated with an application to allow the Retreival Provider to be administered.
* [Retrieval Client](https://github.com/ConsenSys/fc-retrieval-client): A Golang library that can be integrated with an application to allow users to discover which Retrieval Providers can deliver content given a Piece CID.
* [Register](https://github.com/ConsenSys/fc-retrieval-register): A services that emulates an in-built actor. The functionality provided by this service will be incorporated into the Filecoin blockchain node software in a later release. 
* [Integration Tests](https://github.com/ConsenSys/fc-retrieval-itest): The integration test system acts as an application, incorporating the Client, Gateway Admin, and Provider Admin. It runs as a Docker container, along with the Gateway, Provider, and Register to test the system.
* [Common](https://github.com/ConsenSys/fc-retrieval-common): Common Golang packages used by the other components.

## Main Functionality
This release includes functionality to deliver the following work flow:

1. Initialise Gateway using Gateway Admin.
2. Initialise Provider using Provider Admin.
3. The Gateway and Provider discover each other via the Register.
4. Using Provider Admin to ask the Provider to publish a Piece CID Group Offer. The Gateway will receive the offer and store it.
5. Start a Retrieval Client and add the Gateway to the Client manager. The Client discovers the Gateway.
6. Use the Client to retrieve a Piece CID offer from the Gateway that was previously published by the Provider.

## How to Build and Test
To get the release and test it, ensure you have Docker installed and running, have Golang installed, and have standard Linux tools available, and use the following commands:
```
git clone https://github.com/ConsenSys/fc-retrieval-common.git
cd fc-retrieval-common/scripts
bash clonebuildtest.sh 163-poc1-release
```

The script clones all of the required repos, checks them out of the branch 163-poc1-release, checks that the Golang dependancies are up to date, **removes all Docker containers and images** builds the components, and runs the tests by instantiating a Docker Compose network for each test.

The expected test output is shown [here](PoC1_expected_test_output.md).