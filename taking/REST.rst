RESTful

REST: architectural style - not strict standard
use only NOUN, just 2 URLS per resource - one for collection, one for element
base URL simple,intuitive
use HTTP verbs

NOUNS for RESOURCES
=====
    * Use plurar
    * Concrete rather than abstract
    * URL should not deeper than /resource/identifier/resource
    * putting optional states and attributes behind HTTP ? mark:
      GET /dogs?color=red&state=running&location=park

HANDLING ERROR
=====
    * Use HTTP status code : over 70
    * Scene:    sucess - client error - server error
                200     -   400         -   500
    *   201 : created
        304 - not modified
        404 - not found
        401 - unauthorized
        403 - forbidden
    * return msg as verbose as possible - should add link to doc

Versioning
=====
    * always add number version
      - prefix "v", move it to most left as possible
      - use ordinal number, not fractal
    * put number version in header?
      - yes if it change the logic you write to handle the response
      - no if it doesn't change the logic

Partial response, paginate objs in db
=====
    * Return only needed info
    * Use /dogs?fields=name,color,location:group(address, country)
    * /dog?limit=25&offset=50 - and return metadata about total avail records
      - Default: limit=10&offset=0
Response dont involve resources
=====
    * use verb: /convert?from=EUR&to=CNY&amount=100
    * make it clear in doc about non-resources

MultiFORMAT
=====
    * /dog/123.json
    * follow JS conventions for naming attributes
      use CamelCase 

SEARCH
=====
    * Global search: /search?q=hvn+hehe
    * Scoped search: /owners/5678/dogs?q=fulffy+fur
    * formatted search: /search.xml?q=fulffy+fur

SUBDOMAIN
=====
    * Use only 1 subdomain: api.hvn.com

EXCEPTIONS
=====
    * use suppress_response_codes - true
    * put HTTP response code to message
    * support del and update:
      create: /dogs?method=post
      read : /dogs
      update : /dogs/1234?method=put&location=park
      delete : /dogs/1234?method=delete -- DONT USE WITH GET

PATTERN
=====
    * use API facade pattern:



