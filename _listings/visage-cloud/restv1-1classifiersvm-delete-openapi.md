---
swagger: "2.0"
x-collection-name: Visage Cloud
x-complete: 0
info:
  title: Visage Cloud Delete existing classifier
  description: ""
  termsOfService: https://visagecloud.com/terms-of-use
  contact:
    name: VisageCloud
    url: https://visagecloud.com
    email: office@visagecloud.com
  version: "1.1"
host: visagecloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1.1/account/account:
    get:
      summary: Get account information by accessKey and secretKey
      description: ""
      operationId: getAccountByAccessKeyUsingGET
      x-api-path-slug: restv1-1accountaccount-get
      parameters:
      - in: query
        name: accessKey
        description: accessKey
      - in: query
        name: secretKey
        description: secretKey
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/account/billing:
    get:
      summary: Get billing information by accessKey and secretKey
      description: ""
      operationId: getBillingPerAccountUsingGET
      x-api-path-slug: restv1-1accountbilling-get
      parameters:
      - in: query
        name: accessKey
        description: accessKey
      - in: query
        name: dateTemplate
        description: dateTemplate
      - in: query
        name: endDateTime
        description: endDateTime
      - in: query
        name: secretKey
        description: secretKey
      - in: query
        name: startDateTime
        description: startDateTime
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/account/changePassword:
    post:
      summary: Change password for an account using old password
      description: ""
      operationId: changePasswordUsingPOST
      x-api-path-slug: restv1-1accountchangepassword-post
      parameters:
      - in: query
        name: email
        description: email
      - in: query
        name: newPassword
        description: newPassword
      - in: query
        name: oldPassword
        description: oldPassword
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/account/login:
    post:
      summary: Get account information including accessKey and secretKey by email
        and password
      description: ""
      operationId: loginWithEmailUsingPOST
      x-api-path-slug: restv1-1accountlogin-post
      parameters:
      - in: query
        name: email
        description: email
      - in: query
        name: password
        description: password
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/analysis/compare:
    get:
      summary: Compare several faces identified by faceHash, without depending on
        mapping faces to profiles
      description: ""
      operationId: compareFacesUsingGET
      x-api-path-slug: restv1-1analysiscompare-get
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: faceHashes
        description: The IDs of the faces which you want compared, comma-separated
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      - in: query
        name: showDetails
        description: Show details
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/analysis/detection:
    post:
      summary: Perform detection on a given picture or picture URL
      description: ""
      operationId: performAnalysisUsingPOST
      x-api-path-slug: restv1-1analysisdetection-post
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: algorithmVersion
        description: Algorithm version (V2 is more performant but not backward compatible)
      - in: query
        name: filters
        description: '[For advanced users only] Change feature filters for robustness
          of feature extraction'
      - in: query
        name: options
        description: '[For advanced users only] Options for preprocessing of image'
      - in: formData
        name: picture
        description: The multipart/form-data version of the image, in case a direct
          upload is used
      - in: query
        name: pictureURL
        description: The URL of the picture, assuming it is served by a third party
          server
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      - in: query
        name: skipEXIF
        description: Skip EXIF rotation procesing
      - in: query
        name: storeAnalysisPicture
        description: Boolean value indicating whether you want the picture of the
          analysis to be stored for later retrieval
      - in: query
        name: storeFacePictures
        description: Boolean value indicating whether you want the faces inside the
          picture to be stored for later retrieval
      - in: query
        name: storePicture
        description: Boolean value indicating whether you want the original picture
          to be stored for later retrieval
      - in: query
        name: storeResult
        description: Boolean value indicating whether you want the result of the analysis
          to be stored
      - in: query
        name: waitForPictureUpload
        description: Waits until the picture is successfully uploaded, before returning
          the response back the the client
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/analysis/listLatest:
    get:
      summary: Retrieve the last *count* operations per current account
      description: ""
      operationId: retriveLatestUsingGET
      x-api-path-slug: restv1-1analysislistlatest-get
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: count
        description: How many records to retrieve at a time
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/analysis/recognition:
    post:
      summary: Perform labeled recognition on a given picture or picture URL
      description: ""
      operationId: performRecognitionUsingPOST
      x-api-path-slug: restv1-1analysisrecognition-post
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: algorithmVersion
        description: Algorithm version (V2 is more performant but not backward compatible)
      - in: query
        name: attributeFilters
        description: Filters that will be applied on the recognition operation
      - in: query
        name: collectionId
        description: Uniquely identified collection that can store multiple profiles
      - in: query
        name: filters
        description: '[For advanced users only] Change feature filters for robustness
          of feature extraction'
      - in: query
        name: labels
        description: Labels associated with the given picture or picture URL
      - in: query
        name: options
        description: '[For advanced users only] Options for preprocessing of image'
      - in: formData
        name: picture
        description: The picture itself
      - in: query
        name: pictureURL
        description: The URL of the picture
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      - in: query
        name: skipEXIF rotation processing
        description: Skip EXIF rotation procesing
      - in: query
        name: storeAnalysisPicture
        description: Boolean value indicating whether you want the picture of the
          analysis to be stored for later retrieval
      - in: query
        name: storeFacePictures
        description: Boolean value indicating whether you want the faces inside the
          picture to be stored for later retrieval
      - in: query
        name: storePicture
        description: Boolean value indicating whether you want the original picture
          to be stored for later retrieval
      - in: query
        name: storeResult
        description: Boolean value indicating whether you want the result of the analysis
          to be stored
      - in: query
        name: waitForPictureUpload
        description: Waits until the picture is successfully uploaded, before returning
          the response back the the client
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/analysis/retrieve:
    get:
      summary: Retrieve a complete analysis object including both detection and recognition
        information
      description: ""
      operationId: retrieveAnalysisUsingGET
      x-api-path-slug: restv1-1analysisretrieve-get
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: analysisId
        description: The ID of the analysis for which the data will be retrieved
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/analytics/counting:
    post:
      summary: Count individuals in streams or collections
      description: ""
      operationId: counterUsingPOST
      x-api-path-slug: restv1-1analyticscounting-post
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: collectionIds
        description: Collection ids
      - in: query
        name: endDateTime
        description: endDateTime
      - in: query
        name: maxBatchIterations
        description: maxBatchIterations
      - in: query
        name: maxIterations
        description: maxIterations
      - in: query
        name: mergingStep
        description: mergingStep
      - in: query
        name: minNeighborsMergedPerIteration
        description: minNeighborsMergedPerIteration
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      - in: query
        name: shuffling
        description: shuffling
      - in: query
        name: startDateTime
        description: startDateTime
      - in: query
        name: streamIds
        description: Stream Ids
      - in: query
        name: visitDuration
        description: visitDuration
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/analytics/presence/timeseries:
    post:
      summary: Show audience (based on number of occurrences of each person) breakdown
        per declared attribute (age, gender).
      description: ""
      operationId: presenceTimeseriesUsingPOST
      x-api-path-slug: restv1-1analyticspresencetimeseries-post
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: attributes
        description: attributes
      - in: query
        name: endDateTime
        description: endDateTime
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      - in: query
        name: startDateTime
        description: startDateTime
      - in: query
        name: step
        description: step
      - in: query
        name: streamIds
        description: Stream Ids
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/analytics/presence/total:
    post:
      summary: Show presence (based on number of occurences of each face) breakdown
        per declared attribute (age, gender)
      description: ""
      operationId: presenceTotalUsingPOST
      x-api-path-slug: restv1-1analyticspresencetotal-post
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: attributes
        description: attributes
      - in: query
        name: endDateTime
        description: endDateTime
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      - in: query
        name: startDateTime
        description: startDateTime
      - in: query
        name: streamIds
        description: Stream Ids
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/classifier/svm:
    delete:
      summary: Delete existing classifier
      description: ""
      operationId: removeClassiferUsingDELETE
      x-api-path-slug: restv1-1classifiersvm-delete
      parameters:
      - in: query
        name: accessKey
        description: The accessKey provided by VisageCloud
      - in: query
        name: id
        description: The id of the classifier that will be removed
      - in: query
        name: secretKey
        description: The secretKey or readOnlyKey provided by VisageCloud
      responses:
        200:
          description: OK
      tags:
      - ""
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