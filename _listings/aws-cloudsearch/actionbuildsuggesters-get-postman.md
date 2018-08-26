{
  "info": {
    "name": "AWS CloudSearch Build Suggesters",
    "_postman_id": "b44f0bc9-c034-4c26-a9b8-741447f198ec",
    "description": "Indexes the search suggestions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "c9ac739e-4b47-4de1-848f-9bbf090b2090",
          "name": "AddTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?Base=Base&InternalException=InternalException&LimitExceededException=LimitExceededException&ValidationException=ValidationException",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches resource tags to an\n Amazon CloudSearch domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8187c920-82a9-4eb5-9d39-ba38f5898cbf"
            }
          ]
        }
      ]
    },
    {
      "name": "Suggesters",
      "item": [
        {
          "id": "fa54dadc-c00a-4691-9f24-9ef59803b012",
          "name": "BuildSuggesters",
          "request": {
            "url": "http://example.com/api/?Action=BuildSuggesters?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Indexes the search suggestions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2764e6d8-e12a-4627-904a-88cc7b904483"
            }
          ]
        }
      ]
    }
  ]
}