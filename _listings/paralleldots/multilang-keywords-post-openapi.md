---
swagger: "2.0"
x-collection-name: ParallelDots
x-complete: 0
info:
  title: ParallelDots Multilang_Keywords
  description: |-
    # Introduction
    What does your API do?

    Extract Keywords from different languages using this API.

    # Overview
    Things that the developers should know about

    The API accepts the input parameters as form-data.The API works best when input long and multiple sentences.Languages supported are German(de), French(fr), Dutch(nl), Italian(it), Spanish(es), Portuguese(pt), Danish(da), Finish(fi)
    Response will be in JSON as shown below:

    ```
    {
        "keywords": [
            {
                "relevance_score": 4,
                "keyword": "Prime Minister Narendra Modi"
            },
            {
                "relevance_score": 6,
                "keyword": "Human Resource Development Minister Smriti Irani"
            },
            {
                "relevance_score": 2,
                "keyword": "Lok Sabha"
            },
            {
                "relevance_score": 1,
                "keyword": "ongoing"
            },
            {
                "relevance_score": 2,
                "keyword": "JNU row"
            },
            {
                "relevance_score": 2,
                "keyword": "Dalit scholar"
            },
            {
                "relevance_score": 2,
                "keyword": "Rohith Vemula"
            },
            {
                "relevance_score": 3,
                "keyword": "Hyderabad Central University"
            }
        ],
        "usage": "By accessing ParallelDots API or using information generated by ParallelDots API, you are agreeing to be bound by the ParallelDots API Terms of Use: http://www.paralleldots.com/terms-and-conditions"
    }

    ```

    # Authentication
    What is the preferred way of using the API?

    An API key is required to be sent as a parameter to authenticate your requests.


    # Rate limit
    Is there a limit to the number of requests an user can send?

    There is no rate limit as such but too many concurrent requests will throw 504 time-out error from nginx.
  version: 1.0.0
host: apis.paralleldots.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /keywords:
    post:
      summary: Keywords
      description: |-
        # Introduction
        What does your API do?

        Keyword Generator are powerful tools in text analysis that can be used to index data, generate tag clouds and accelerate the searching time. It generates an extensive list of relevant keywords and phrases to make research more context focussed.

        # Overview
        Things that the developers should know about

        The API accepts the input parameters as form-data.

        Response will be in JSON as shown below:

        ```
        {
            "keywords": [
                {
                    "keyword": "Cristiano Ronaldo",
                    "confidence_score": 0.887065
                },
                {
                    "keyword": "Principality Stadium",
                    "confidence_score": 0.903289
                },
                {
                    "keyword": "Cardiff last",
                    "confidence_score": 0.806802
                },
                {
                    "keyword": "couple",
                    "confidence_score": 0.69036
                },
                {
                    "keyword": "hours",
                    "confidence_score": 0.984956
                },
                {
                    "keyword": "Real Madrid win",
                    "confidence_score": 0.812151
                }
            ],
            "usage": "By accessing ParallelDots API or using information generated by ParallelDots API, you are agreeing to be bound by the ParallelDots API Terms of Use: http://www.paralleldots.com/terms-and-conditions"
        }
        ```

        # Authentication
        What is the preferred way of using the API?

        An API key is required to be sent as a parameter to authenticate your requests.


        # Rate limit
        Is there a limit to the number of requests an user can send?

        There is no rate limit as such but too many concurrent requests will throw 504 time-out error from nginx.
      operationId: KeywordsPost
      x-api-path-slug: keywords-post
      parameters:
      - in: formData
        name: api_key
      - in: formData
        name: text
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Keywords
      - Analysis
  /multilang_keywords:
    post:
      summary: Multilang_Keywords
      description: |-
        # Introduction
        What does your API do?

        Extract Keywords from different languages using this API.

        # Overview
        Things that the developers should know about

        The API accepts the input parameters as form-data.The API works best when input long and multiple sentences.Languages supported are German(de), French(fr), Dutch(nl), Italian(it), Spanish(es), Portuguese(pt), Danish(da), Finish(fi)
        Response will be in JSON as shown below:

        ```
        {
            "keywords": [
                {
                    "relevance_score": 4,
                    "keyword": "Prime Minister Narendra Modi"
                },
                {
                    "relevance_score": 6,
                    "keyword": "Human Resource Development Minister Smriti Irani"
                },
                {
                    "relevance_score": 2,
                    "keyword": "Lok Sabha"
                },
                {
                    "relevance_score": 1,
                    "keyword": "ongoing"
                },
                {
                    "relevance_score": 2,
                    "keyword": "JNU row"
                },
                {
                    "relevance_score": 2,
                    "keyword": "Dalit scholar"
                },
                {
                    "relevance_score": 2,
                    "keyword": "Rohith Vemula"
                },
                {
                    "relevance_score": 3,
                    "keyword": "Hyderabad Central University"
                }
            ],
            "usage": "By accessing ParallelDots API or using information generated by ParallelDots API, you are agreeing to be bound by the ParallelDots API Terms of Use: http://www.paralleldots.com/terms-and-conditions"
        }

        ```

        # Authentication
        What is the preferred way of using the API?

        An API key is required to be sent as a parameter to authenticate your requests.


        # Rate limit
        Is there a limit to the number of requests an user can send?

        There is no rate limit as such but too many concurrent requests will throw 504 time-out error from nginx.
      operationId: MultilangKeywordsPost
      x-api-path-slug: multilang-keywords-post
      parameters:
      - in: formData
        name: api_key
      - in: formData
        name: lang_code
      - in: formData
        name: text
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Multilang_Keywords
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---