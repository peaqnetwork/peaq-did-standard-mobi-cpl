# peaq-did-standard-mobi-cpl
Peaq DID standard for MOBI compliance 

## Introduction
The peaq VID standard supports all types of vehicles and enables them to discover each other, carry out transactions, verify claims, preserve privacy and  remain sovereign. The standard aims to optimize any web3 use case in the vehicle mobility sector. The standard is compliant with the MOBI VID standard which is supported by diverse industry leaders with the goal to provide a standard interfaces for discovery which allows two participants to successfully engage in a transaction.

## Status of the document
This document is currently in draft stage and is the first iteration of the peaq VID which provisions means to enable successful on-boarding and commercial operations related to vehicles and vehicle charging stations.
This is a foundation draft and will be refined to accommodate additional use cases in forthcoming iteractions to make this DID standard more generic and robust by taking into account the learnt lessons.
In coming iterations to this document, references to charging stations will be generalized to reflect machines. 

# json of Peaq DID standard for MOBI compliance 
```json
{
  "id": "did:peaq:5H3QUhRvdgzNGYzvzgQtKyTyvGv8Vz6SwQq6v7aGWZiGJWpf",
  "verificationMethod": [
    {
      "id": "a8c581471e4bc5ab6e7f7ca87781d350d337645917d2fce173009ca3e9dab98b",
      "type": "Ed25519VerificationKey2020",
      "controller": "did:peaq:5H3QUhRvdgzNGYzvzgQtKyTyvGv8Vz6SwQq6v7aGWZiGJWpf",
      "publicKeyMultibase": "5FszaBvMn8dSNvmPY3zxT4bHdKpZaccTKwsYSBLwT5C6z8Tf"
    },
    {
      "id": "dc2f6b696de92807498cb018eab92f98addc137fc8aab0ef92db751747f8e33d", 
      "type": "Sr25519VerificationKey2020", 
      "controller": "did:peaq:5H3QUhRvdgzNGYzvzgQtKyTyvGv8Vz6SwQq6v7aGWZiGJWpf", 
      "publicKeyMultibase": "5H3QUhRvdgzNGYzvzgQtKyTyvGv8Vz6SwQq6v7aGWZiGJWpf", 
    }
  ],
  "signature": {
    "type": "Sr25519VerificationKey2020",
    "issuer": "<did address of Peaq>",
    "hash": "<signature>"
  },
  "service": [
    {
      "id": "5H3QUhRvdgzNGYzvzgQtKyTyvGv8Vz6SwQq6v7aGWZiGJWpf", 
      "type": "payment", 
      "serviceEndpoint": "5H3QUhRvdgzNGYzvzgQtKyTyvGv8Vz6SwQq6v7aGWZiGJWpf", 
    },
    {
      "id": "5H3QUhRvdgzNGYzvzgQtKyTyvGv8Vz6SwQq6v7aGWZiGJWpf", 
      "type": "p2p", 
      "serviceEndpoint": "/ip4/127.0.0.1/tcp/10333/p2p/12D3KooWCazx4ZLTdrA1yeTTmCy5sGW32SFejztJTGdSZwnGf5gh", 
    }, 
    {
      "id": "MOBI",
      "type": "EV",
      "document": {
        "uvi": "mobi:uvi:1234567890",
        "engine_serial_number": "1234567890",
        "engine_code": 123456,
        "Color": "White",
        "CountryOfOrigin": "Germany",
        "DateOfProduction": "220326",
        "EngineCode": "WBS0",
        "EngineSerialNumber": "5661",
        "FuelType": "1",
        "Issuer": "Tesla",
        "Manufacturer": "BMW",
        "Model": "X6",
        "ModelYear": "2012",
        "PlantCode": "009",
        "PreviousVBC": "778",
        "TransmissionSerialNumber": "1231",
        "TrimType": "331"
      }
    }
  ]
}
```
