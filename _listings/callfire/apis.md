---
name: CallFire
x-slug: callfire
description: CallFire is a cloud-based telephony company that provides voice and text
  connectivity services. It offers the necessary tools for businesses to communicate
  and market effectively. The company works to provide a diverse line of innovative
  products that enable its users to get their messages delivered.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Keywords
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/apis.md
specificationVersion: "0.14"
apis:
- name: Callfire Find keywords
  x-api-slug: callfire
  description: Searches for all keywords available for purchase on the CallFire platform.
    If a keyword appears in the response, it is available for purchase. List the 'keywords'
    in a query parameter to search for multiple keywords (at least one keyword should
    be sent in request)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords
  tags: Keywords
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/keywords-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/keywords-get-openapi.md
- name: Callfire Find keyword leases
  x-api-slug: callfire
  description: Searches for all keywords owned by user. A keyword lease is the ownership
    information involving a keyword
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords/leases
  tags: Keywords,Leases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/keywordsleases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/keywordsleases-get-openapi.md
- name: Callfire Find a specific lease
  x-api-slug: callfire
  description: Searches for all keywords owned by user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords/leases/{keyword}
  tags: Keywords,Leases,Keyword
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/keywordsleaseskeyword-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/keywordsleaseskeyword-get-openapi.md
- name: Callfire Update a lease
  x-api-slug: callfire
  description: Updates a keyword lease. Turns the autoRenew on/off.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords/leases/{keyword}
  tags: Keywords,Leases,Keyword
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/keywordsleaseskeyword-put-openapi.md
- name: Callfire Check for a specific keyword
  x-api-slug: callfire
  description: Searches for the specific keyword to purchase on the CallFire platform.
    Returns 'true' if keyword is available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords/{keyword}/available
  tags: Keywords,Keyword,Available
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/keywordskeywordavailable-get-openapi.md
- name: Callfire Purchase keywords
  x-api-slug: callfire
  description: Purchase keywords. Send a list of available keywords into this API
    to purchase them using CallFire credits. Make sure the account has enough credits
    before trying to purchase the keywords
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//orders/keywords
  tags: Orders,Keywords
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/orderskeywords-post-openapi.md
- name: Callfire
  x-api-slug: callfire
  description: CallFire is a cloud-based telephony company that provides voice and
    text connectivity services. It offers the necessary tools for businesses to communicate
    and market effectively. The company works to provide a diverse line of innovative
    products that enable its users to get their messages delivered.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2
  tags: Keywords
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/callfire/openapi.md
x-common:
- type: x-net-sdk
  url: https://github.com/CallFire/CallFire-CSharp-SDK
- type: x-account-billing
  url: https://answers.callfire.com/hc/en-us/sections/200166268-Billing
- type: x-account-settings
  url: https://answers.callfire.com/hc/en-us/sections/200187056-Account-Settings
- type: x-authentication
  url: https://www.callfire.com/api-documentation/how-do-i-enable-api-on-my-account
- type: x-blog
  url: https://www.callfire.com/blog
- type: x-blog-rss
  url: https://www.callfire.com/blog/feed
- type: x-twitter
  url: https://twitter.com/CallFire
- type: x-case-studies
  url: https://www.callfire.com/case-studies
- type: x-compliance
  url: https://www.callfire.com/legal/compliance
- type: x-contact-form
  url: https://www.callfire.com/contact
- type: x-crunchbase
  url: https://www.crunchbase.com/organization/callfire
- type: x-developer
  url: https://www.callfire.com/api-documentation
- type: x-documentation
  url: https://www.callfire.com/api-documentation/rest/version/1.1
- type: x-drupal-plugin
  url: https://github.com/CallFire/CallFire-Drupal-Integration
- type: x-email
  url: support@callfire.com
- type: x-facebook
  url: https://www.facebook.com/callfire
- type: x-faq
  url: https://answers.callfire.com/hc/en-us/sections/200193833-FAQs
- type: x-getting-started
  url: https://www.callfire.com/help/docs/getting-started
- type: x-github
  url: https://github.com/callfire
- type: x-glossary
  url: https://www.callfire.com/help/glossary/communications
- type: x-google-plus
  url: https://plus.google.com/100142045997033051154
- type: x-messages
  url: https://www.callfire.com/ui/number/messages?6
- type: x-partners
  url: https://www.callfire.com/partners
- type: x-phone
  url: 1.877.897.3473
- type: x-php-sdk
  url: https://github.com/CallFire/CallFire-PHP-SDK
- type: x-pricing
  url: https://www.callfire.com/pricing
- type: x-privacy
  url: https://www.callfire.com/legal/privacy
- type: x-selfservice-registration
  url: https://www.callfire.com/ui/register?1
- type: x-terms-of-service
  url: https://www.callfire.com/legal/terms
- type: x-tickets
  url: https://answers.callfire.com/hc/en-us/requests/new
- type: x-tour
  url: javascript:;
- type: x-videos
  url: https://answers.callfire.com/hc/en-us/articles/200849247-Videos
- type: x-webinars
  url: https://answers.callfire.com/hc/en-us/articles/202174798-Webinars
- type: x-website
  url: http://www.callfire.com
- type: x-wordpress-plugin
  url: https://github.com/CallFire/CallFire-WordPress-Integration
- type: x-youtube
  url: https://www.youtube.com/user/CallFireTelephony
- type: x-zapier
  url: https://zapier.com/zapbook/callfire/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---