{
  "info": {
    "name": "AWS CloudSearch Delete Suggester",
    "_postman_id": "187b3475-7289-44a3-b54f-2231bf0f2b9e",
    "description": "Deletes a suggester.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "9e4ce384-b68b-48aa-818d-304c91b2369b",
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
              "id": "d97f5027-c599-403e-afa6-f814823fea06"
            }
          ]
        }
      ]
    },
    {
      "name": "Suggesters",
      "item": [
        {
          "id": "0efe2a8b-79f8-4390-8fd5-10b4c5ff1476",
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
              "id": "03fe223c-f7a5-4b2b-aedb-bdbef5a69747"
            }
          ]
        },
        {
          "id": "c39c0467-c1b6-403c-a1f0-bc52320a60ed",
          "name": "DefineSuggester",
          "request": {
            "url": "http://example.com/api/?Action=DefineSuggester?DomainName=DomainName&Suggester=Suggester",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures a suggester for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "697b4229-4d7c-43b8-9794-3821cf5da02a"
            }
          ]
        },
        {
          "id": "6df8c6b0-2921-4d0d-8dc6-7fcf8109220f",
          "name": "DeleteSuggester",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSuggester?DomainName=DomainName&SuggesterName=SuggesterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a suggester."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99809efa-1e6d-4ecb-8620-19bd52f46612"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "6bb5972e-f9e5-4416-a73f-741d658f1ea1",
          "name": "CreateDomain",
          "request": {
            "url": "http://example.com/api/?Action=CreateDomain?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bb4ba85-3242-414c-9061-530a461a651f"
            }
          ]
        },
        {
          "id": "3b2220f6-86c3-4218-85df-9e2edef503c7",
          "name": "DeleteDomain",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDomain?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Permanently deletes a search domain and all of its data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8727e29f-2c01-40c3-bc24-473bc09b6f4a"
            }
          ]
        }
      ]
    },
    {
      "name": "Analysis Scheme",
      "item": [
        {
          "id": "c511aa29-83f4-4ff4-a1cf-13b70c0a6788",
          "name": "DefineAnalysisScheme",
          "request": {
            "url": "http://example.com/api/?Action=DefineAnalysisScheme?AnalysisScheme=AnalysisScheme&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an analysis scheme that can be applied to a text or text-array field to define language-specific text processing options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29f9db7f-7c0b-4c14-9439-76ec7fd29cda"
            }
          ]
        },
        {
          "id": "7b5f7dd7-c1e7-415e-8ff1-8de6fe17cabc",
          "name": "DeleteAnalysisScheme",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAnalysisScheme?AnalysisSchemeName=AnalysisSchemeName&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an analysis scheme."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e0d0329-5d9b-4945-b9a3-f870c746bdd4"
            }
          ]
        }
      ]
    },
    {
      "name": "Expressions",
      "item": [
        {
          "id": "13fa9b70-a2e8-403b-82c9-45bf6bff10bf",
          "name": "DefineExpression",
          "request": {
            "url": "http://example.com/api/?Action=DefineExpression?DomainName=DomainName&Expression=Expression",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an Expression  for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0453f6dd-3c37-4dcb-a3cd-6ea65fbc9eef"
            }
          ]
        },
        {
          "id": "91df418e-17b2-4cf7-869c-e23aa64240ec",
          "name": "DeleteExpression",
          "request": {
            "url": "http://example.com/api/?Action=DeleteExpression?DomainName=DomainName&ExpressionName=ExpressionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an \n  Expression\n  from the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6562d14-ae05-4e1f-aa3a-cf2d0b1bf2d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Index Fields",
      "item": [
        {
          "id": "eb665ca4-b563-411b-b426-f7b5f5c90788",
          "name": "DefineIndexField",
          "request": {
            "url": "http://example.com/api/?Action=DefineIndexField?DomainName=DomainName&IndexField=IndexField",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an ndexField  for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb101f9d-4996-434a-b9a5-e7fa3f98e21d"
            }
          ]
        },
        {
          "id": "e5ca05a6-ff11-4edb-9fb8-5d549808cacd",
          "name": "DeleteIndexField",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIndexField?DomainName=DomainName&IndexFieldName=IndexFieldName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an \n  IndexField\n  from the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4685dc14-dfe4-4203-aece-8ff53241414e"
            }
          ]
        }
      ]
    }
  ]
}