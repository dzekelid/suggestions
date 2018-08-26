{
  "info": {
    "name": "AWS CloudSearch Describe Suggesters",
    "_postman_id": "5205b11c-d77c-488e-8613-86aed5963f31",
    "description": "Gets the suggesters configured for a domain.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "81d4649b-b506-4fc2-8d46-7ef2bedf8435",
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
              "id": "89cc52f4-24f0-4c4b-80f5-94c06f08c9ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Suggesters",
      "item": [
        {
          "id": "408979cb-ba33-467b-bac8-97827a65f259",
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
              "id": "d615d67b-be8f-4cbe-bb07-22e69f1fa74e"
            }
          ]
        },
        {
          "id": "0c01f7f3-d7c7-42f2-a4d5-1ed035a311ec",
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
              "id": "bdc803a5-91d3-428b-b934-32f847f64281"
            }
          ]
        },
        {
          "id": "96712998-1ede-40d1-87a9-2570605d746d",
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
              "id": "0b86fc96-9a4a-41bf-a492-827988f7afb1"
            }
          ]
        },
        {
          "id": "441f5528-ded8-4667-aef7-7d82acf6cd2b",
          "name": "DescribeSuggesters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSuggesters?Deployed=Deployed&DomainName=DomainName&SuggesterNames.member.N=SuggesterNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the suggesters configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b568674-1648-427b-98a1-de380e6571fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "e2020911-f501-467d-831b-e20b24537094",
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
              "id": "1d22c893-a9a3-4d5b-b43a-8de2a994242e"
            }
          ]
        },
        {
          "id": "c605e75c-4708-47a9-9026-63231e50cf9e",
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
              "id": "210afa34-6e91-49de-933a-26fa06a6a1c4"
            }
          ]
        },
        {
          "id": "0280449f-e717-49e9-ac36-d5dad090c044",
          "name": "DescribeDomains",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDomains?DomainNames.member.N=DomainNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the search domains owned by this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16a9bc78-6a96-473a-8bf4-1f289e4a7234"
            }
          ]
        }
      ]
    },
    {
      "name": "Analysis Scheme",
      "item": [
        {
          "id": "1571fcc8-1987-45f0-87a6-a44d64988edb",
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
              "id": "f1a37878-52ba-4e7c-9283-fcec81844329"
            }
          ]
        },
        {
          "id": "bc0d14f9-f68c-4168-8ffa-3467950e1bf0",
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
              "id": "f8858ac6-3386-4faa-9cc0-d8100784db6a"
            }
          ]
        },
        {
          "id": "f8a41581-db04-4bef-be98-98f4dacfab95",
          "name": "DescribeAnalysisSchemes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAnalysisSchemes?AnalysisSchemeNames.member.N=AnalysisSchemeNames.member.N&Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the analysis schemes configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "809b5ca7-5abd-4d99-ac75-dc73173cfaed"
            }
          ]
        }
      ]
    },
    {
      "name": "Expressions",
      "item": [
        {
          "id": "a63038db-cc68-4c00-9fa6-988c0418975f",
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
              "id": "7f364142-bc2e-4328-b7d0-03e669af4a11"
            }
          ]
        },
        {
          "id": "3b003142-74ea-4e04-95e0-453512f66e49",
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
              "id": "9ba6bae1-2ee5-434a-b6bb-daea8f3b95f4"
            }
          ]
        },
        {
          "id": "c0d999da-2572-4493-a1b1-37f0e996c739",
          "name": "DescribeExpressions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeExpressions?Deployed=Deployed&DomainName=DomainName&ExpressionNames.member.N=ExpressionNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the expressions configured for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ef0245f-83ee-4306-84e4-eded430690f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Index Fields",
      "item": [
        {
          "id": "f17ea040-98d3-4378-a2dd-62ad3bbce205",
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
              "id": "124acc55-cd4d-40cf-a37e-d88d0982efe3"
            }
          ]
        },
        {
          "id": "f0a3f245-5889-4b2c-91cb-5e112f94ae67",
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
              "id": "c1e3fb7f-4ca0-4230-a296-8f3caff012df"
            }
          ]
        },
        {
          "id": "65ae94e5-fe10-4cd5-a228-8667aa8b359b",
          "name": "DescribeIndexFields",
          "request": {
            "url": "http://example.com/api/?Action=DescribeIndexFields?Deployed=Deployed&DomainName=DomainName&FieldNames.member.N=FieldNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the index fields configured for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0c614b1-a0e7-4d70-8b95-0a4ebbd232e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Availability Options",
      "item": [
        {
          "id": "ac8fa948-5275-4454-b03b-83d9f29471b1",
          "name": "DescribeAvailabilityOptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailabilityOptions?Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the availability options configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "750fb0a5-5064-4729-ac4c-94280bfcf0ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Parameters",
      "item": [
        {
          "id": "334d385a-bb56-4cd2-ae7f-17a776bb94c5",
          "name": "DescribeScalingParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScalingParameters?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the scaling parameters configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af2adff8-5f87-407f-8789-3476fb4ee49d"
            }
          ]
        }
      ]
    },
    {
      "name": "Service Access Policies",
      "item": [
        {
          "id": "cd86528c-3a7c-4d30-a3e9-0b9b7a5636a8",
          "name": "DescribeServiceAccessPolicies",
          "request": {
            "url": "http://example.com/api/?Action=DescribeServiceAccessPolicies?Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the access policies that control access to the domain's document and search endpoints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c00350b-4234-4e76-b701-798952bce5c4"
            }
          ]
        }
      ]
    }
  ]
}