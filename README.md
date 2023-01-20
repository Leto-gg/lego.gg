# Leto.gg/lookup HTTP API
This repo is dedicated to the public endpoint of leto.gg. This repo consists of the main website as well as an example set of API code to retrieve the number of requests of an IPFS CID/BAFY via the leto engine found [here](https://github.com/noryev/leto-engine)

# Table of Contents
- [Usage](#usage)
- [Development](#development)
- [Setup](#setup)
- [Contributing](#contributing)
- [License](#license)

# Usage

 This is an example of how to make a GET request to the "https://leto.gg/lookup" endpoint with your API, passing an IPFS CID hash as a query parameter:
1. Make sure you have the necessary dependencies installed/imported in your project, such as axios or request.
2. Create a function to make the GET request to the "https://leto.gg/lookup" endpoint and pass the CID hash as a query parameter. The function should take in the CID hash as an argument.

       async function getCID(cid) {
       try {
       const response = await axios.get(https://leto.gg/lookup?cid=${cid});
       return response.query;
       }
  
       catch (error) {
       console.error(error);
       }
       }

3. Call the function and pass in the CID hash as an argument.

       const cid = 'Qm...'; // replace with the actual CID hash
       const query = getCID(cid);
       console.log(query);

4. The response will contain the data associated with the CID hash.


# Development

Currently our implementation is through Elasic Observability for log parsing and were using S3 for hosting the public endpoint 

Currently https://leto.gg redirects to lookup.leto.gg(UI setup to interact with the Leto.gg API-Endpoint)

Elastic Configuration

# Setup

# License
MIT + Apache 2.0
