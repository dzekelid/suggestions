---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 1
info:
  title: Stack Exchange
  description: stack-exchange-is-a-network-of-130-qa-communities-including-stack-overflow-
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/suggested-edits:
    get:
      summary: Suggested Edits
      description: "Returns the suggested edits the user identified by access_token
        has submitted.\n \nThis method returns a list of suggested-edits."
      operationId: returns-the-suggested-edits-the-user-identified-by-access-token-has-submitted-this-method-returns-a-
      x-api-path-slug: mesuggestededits-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Suggested Edits
  /posts/{ids}/suggested-edits:
    get:
      summary: Get Posts Suggested Edits
      description: "Returns suggsted edits on the posts identified in ids.\n \n -
        creation - creation_date\n - approval - approval_date\n - rejection - rejection_date\n
        \ creation is the default sort.\n \n {ids} can contain up to 100 semicolon
        delimited ids, to find ids programatically look for post_id, answer_id, or
        question_id on post, answer, and question objects respectively.\n \nThis method
        returns a list of suggested-edits."
      operationId: returns-suggsted-edits-on-the-posts-identified-in-ids---creation--creation-date--approval--approval-
      x-api-path-slug: postsidssuggestededits-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Suggested Edits
  /suggested-edits:
    get:
      summary: Get Suggested Edits
      description: "Returns all the suggested edits in the systems.\n \nThis method
        returns a list of suggested-edits.\n \nThe sorts accepted by this method operate
        on the follow fields of the suggested_edit object:\n - creation - creation_date\n
        - approval - approval_date Does not return unapproved suggested_edits\n -
        rejection - rejection_date Does not return unrejected suggested_edits\n  creation
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate."
      operationId: returns-all-the-suggested-edits-in-the-systems-this-method-returns-a-list-of-suggestededits-the-sort
      x-api-path-slug: suggestededits-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Suggested Edits
  /suggested-edits/{ids}:
    get:
      summary: Get Suggested Edit
      description: "Returns suggested edits identified in ids.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for suggested_edit_id
        on suggested_edit objects.\n \nThe sorts accepted by this method operate on
        the follow fields of the suggested_edit object:\n - creation - creation_date\n
        - approval - approval_date Does not return unapproved suggested_edits\n -
        rejection - rejection_date Does not return unrejected suggested_edits\n  creation
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of suggested-edits."
      operationId: returns-suggested-edits-identified-in-ids-ids-can-contain-up-to-100-semicolon-delimited-ids-to-find-
      x-api-path-slug: suggestededitsids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Suggested Edits
  /users/{ids}/suggested-edits:
    get:
      summary: Get User Suggested Edits
      description: "Returns the suggested edits a users in {ids} have submitted.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the suggested_edit object:\n -
        creation - creation_date\n - approval - approval_date Does not return unapproved
        suggested_edits\n - rejection - rejection_date Does not return unrejected
        suggested_edits\n  creation is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of suggested-edits."
      operationId: returns-the-suggested-edits-a-users-in-ids-have-submitted-ids-can-contain-up-to-100-semicolon-delimi
      x-api-path-slug: usersidssuggestededits-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Suggested Edits
---