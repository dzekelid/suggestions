---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You dont have to read through a lot of discussion to find the best answer.    Like
  to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Suggestions
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange - Suggested Edits
  x-api-slug: mesuggestededits-get
  description: "Returns the suggested edits the user identified by access_token has
    submitted.\n \nThis method returns a list of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/mesuggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/mesuggestededits-get-openapi.md
- name: Stack Exchange - Get Posts Suggested Edits
  x-api-slug: postsidssuggestededits-get
  description: "Returns suggsted edits on the posts identified in ids.\n \n - creation
    - creation_date\n - approval - approval_date\n - rejection - rejection_date\n
    \ creation is the default sort.\n \n {ids} can contain up to 100 semicolon delimited
    ids, to find ids programatically look for post_id, answer_id, or question_id on
    post, answer, and question objects respectively.\n \nThis method returns a list
    of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/postsidssuggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/postsidssuggestededits-get-openapi.md
- name: Stack Exchange - Get Suggested Edits
  x-api-slug: suggestededits-get
  description: "Returns all the suggested edits in the systems.\n \nThis method returns
    a list of suggested-edits.\n \nThe sorts accepted by this method operate on the
    follow fields of the suggested_edit object:\n - creation - creation_date\n - approval
    - approval_date Does not return unapproved suggested_edits\n - rejection - rejection_date
    Does not return unrejected suggested_edits\n  creation is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/suggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/suggestededits-get-openapi.md
- name: Stack Exchange - Get Suggested Edit
  x-api-slug: suggestededitsids-get
  description: "Returns suggested edits identified in ids.\n \n{ids} can contain up
    to 100 semicolon delimited ids, to find ids programatically look for suggested_edit_id
    on suggested_edit objects.\n \nThe sorts accepted by this method operate on the
    follow fields of the suggested_edit object:\n - creation - creation_date\n - approval
    - approval_date Does not return unapproved suggested_edits\n - rejection - rejection_date
    Does not return unrejected suggested_edits\n  creation is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/suggestededitsids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/suggestededitsids-get-openapi.md
- name: Stack Exchange - Get User Suggested Edits
  x-api-slug: usersidssuggestededits-get
  description: "Returns the suggested edits a users in {ids} have submitted.\n \n{ids}
    can contain up to 100 semicolon delimited ids, to find ids programatically look
    for user_id on user or shallow_user objects.\n \nThe sorts accepted by this method
    operate on the follow fields of the suggested_edit object:\n - creation - creation_date\n
    - approval - approval_date Does not return unapproved suggested_edits\n - rejection
    - rejection_date Does not return unrejected suggested_edits\n  creation is the
    default sort.\n \n It is possible to create moderately complex queries using sort,
    min, max, fromdate, and todate.\n \nThis method returns a list of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/usersidssuggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/usersidssuggestededits-get-openapi.md
- name: Stack Exchange - Suggested Edits
  x-api-slug: mesuggestededits-get
  description: "Returns the suggested edits the user identified by access_token has
    submitted.\n \nThis method returns a list of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/mesuggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/mesuggestededits-get-openapi.md
- name: Stack Exchange - Get Posts Suggested Edits
  x-api-slug: postsidssuggestededits-get
  description: "Returns suggsted edits on the posts identified in ids.\n \n - creation
    - creation_date\n - approval - approval_date\n - rejection - rejection_date\n
    \ creation is the default sort.\n \n {ids} can contain up to 100 semicolon delimited
    ids, to find ids programatically look for post_id, answer_id, or question_id on
    post, answer, and question objects respectively.\n \nThis method returns a list
    of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/postsidssuggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/postsidssuggestededits-get-openapi.md
- name: Stack Exchange - Get Suggested Edits
  x-api-slug: suggestededits-get
  description: "Returns all the suggested edits in the systems.\n \nThis method returns
    a list of suggested-edits.\n \nThe sorts accepted by this method operate on the
    follow fields of the suggested_edit object:\n - creation - creation_date\n - approval
    - approval_date Does not return unapproved suggested_edits\n - rejection - rejection_date
    Does not return unrejected suggested_edits\n  creation is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/suggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/suggestededits-get-openapi.md
- name: Stack Exchange - Get Suggested Edit
  x-api-slug: suggestededitsids-get
  description: "Returns suggested edits identified in ids.\n \n{ids} can contain up
    to 100 semicolon delimited ids, to find ids programatically look for suggested_edit_id
    on suggested_edit objects.\n \nThe sorts accepted by this method operate on the
    follow fields of the suggested_edit object:\n - creation - creation_date\n - approval
    - approval_date Does not return unapproved suggested_edits\n - rejection - rejection_date
    Does not return unrejected suggested_edits\n  creation is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/suggestededitsids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/suggestededitsids-get-openapi.md
- name: Stack Exchange - Get User Suggested Edits
  x-api-slug: usersidssuggestededits-get
  description: "Returns the suggested edits a users in {ids} have submitted.\n \n{ids}
    can contain up to 100 semicolon delimited ids, to find ids programatically look
    for user_id on user or shallow_user objects.\n \nThe sorts accepted by this method
    operate on the follow fields of the suggested_edit object:\n - creation - creation_date\n
    - approval - approval_date Does not return unapproved suggested_edits\n - rejection
    - rejection_date Does not return unrejected suggested_edits\n  creation is the
    default sort.\n \n It is possible to create moderately complex queries using sort,
    min, max, fromdate, and todate.\n \nThis method returns a list of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/usersidssuggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/suggestions/master/_listings/stack-exchange/usersidssuggestededits-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://square.api.gallery.streamdata.io
- type: x-api-stack
  url: http://stack.exchange.stack.network
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-linkedin
  url: https://www.linkedin.com/company/stack-exchange
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---