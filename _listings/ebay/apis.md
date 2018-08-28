---
name: eBay
x-slug: ebay
description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
  goods, digital cameras, baby items, coupons, and everything else on eBay, the worlds
  online marketplace
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
x-kinRank: "8"
x-alexaRank: "42"
tags: Suggestions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/ebay/apis.md
specificationVersion: "0.14"
apis:
- name: Ebay - Get Category Tree Category Tree  Get Category Suggestions
  x-api-slug: category-treecategory-tree-idget-category-suggestions-get
  description: 'This call returns an array of category tree leaf nodes in the specified
    category tree that are considered by eBay to most closely correspond to the query
    string q. Returned with each suggested node is a localized name for that category
    (based on the Accept-Language header specified for the call), and details about
    each of the category''s ancestor nodes, extending from its immediate parent up
    to the root of the category tree. Note: This call can return a large payload,
    so you are advised to submit the request with the following HTTP header: &nbsp;&nbsp;Accept-Encoding:
    application/gzip With this header (in addition to the required headers described
    under HTTP Request Headers), the call returns the response with gzip compression.
    You identify the tree using the category_tree_id parameter, which was returned
    by the getDefaultCategoryTreeId call in the categoryTreeId field. Important: This
    call is not supported in the Sandbox environment. It will return a response payload
    in which the categoryName fields contain random or boilerplate text regardless
    of the query submitted.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/ebay/category-treecategory-tree-idget-category-suggestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/ebay/category-treecategory-tree-idget-category-suggestions-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://easycron.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ebay.stack.network
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-crunchbase
  url: https://crunchbase.com/organization/leah
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-email
  url: spam@ebay.com
- type: x-email
  url: spoof@ebay.com
- type: x-github
  url: https://github.com/eBayDeveloper
- type: x-twitter
  url: https://twitter.com/eBay
- type: x-twitter
  url: https://twitter.com/ebaydev
- type: x-website
  url: https://ebay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---