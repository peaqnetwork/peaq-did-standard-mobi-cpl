# peaq-did-standard-mobi-cpl
Peaq DID standard for MOBI compliance 

# json of Peaq DID standard for MOBI compliance 
{
  "id": "did:peaq:5HRNr4pXH7PYKEmeW1jzJVxepXyg8w2Q3YpgRNHpH8foNr5i",
  "verificationMethod": [
    {
      "id": "#pk1",
      "type": "Ed25519VerificationKey2020",
      "controller": "did:peaq:5HRNr4pXH7PYKEmeW1jzJVxepXyg8w2Q3YpgRNHpH8foNr5i",
      "publicKeyMultibase": "z5HRNr4pXH7PYKEmeW1jzJVxepXyg8w2Q3YpgRNHpH8foNr5i"
    }
  ],
  "signature": {
    "type": "Ed25519VerificationKey2020",
    "issuer": "<did address of Peaq>",
    "hash": "<signature>"
  },
  "service": [
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
