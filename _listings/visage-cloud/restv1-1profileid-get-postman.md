{
  "info": {
    "name": "Visage Cloud Retrieves a profile",
    "_postman_id": "38c96207-42ca-4d8f-b05e-3877804b7bd2",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "bc9c2c7b-41e4-48d3-ba54-93b94a226350",
      "name": "getAccountByAccessKeyUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/account/account?accessKey=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get account information by accessKey and secretKey"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "734f72fe-bd98-4c3d-8019-1767e66d41eb"
        }
      ]
    },
    {
      "id": "69d7dd71-956d-4010-a179-ae448709c3b7",
      "name": "getBillingPerAccountUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/account/billing?accessKey=%7B%7D&dateTemplate=%7B%7D&endDateTime=%7B%7D&secretKey=%7B%7D&startDateTime=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get billing information by accessKey and secretKey"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "3c3a59bb-2587-441b-bf4c-cbb35463abf5"
        }
      ]
    },
    {
      "id": "595f25ef-be51-476f-b0dd-ddcaf00fceb9",
      "name": "changePasswordUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/account/changePassword?email=%7B%7D&newPassword=%7B%7D&oldPassword=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Change password for an account using old password"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d5bce603-0f2d-4446-ab90-b05e9653e7e6"
        }
      ]
    },
    {
      "id": "c394bc63-c97d-49ba-8479-f7bbc7cf4cab",
      "name": "loginWithEmailUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/account/login?email=%7B%7D&password=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get account information including accessKey and secretKey by email and password"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "eba5b300-99ed-4468-a45b-7360d75877cf"
        }
      ]
    },
    {
      "id": "a90f5c39-de4e-43f5-9321-989b6d4481f9",
      "name": "compareFacesUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/analysis/compare?accessKey=%7B%7D&faceHashes=%7B%7D&secretKey=%7B%7D&showDetails=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Compare several faces identified by faceHash, without depending on mapping faces to profiles"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "35b0e0b0-3e5b-4a29-986d-6e20b6d3c5b9"
        }
      ]
    },
    {
      "id": "2413b32c-3777-4afa-a390-67dfe75bf43b",
      "name": "performAnalysisUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/analysis/detection?accessKey=%7B%7D&algorithmVersion=%7B%7D&filters=%7B%7D&options=%7B%7D&pictureURL=%7B%7D&secretKey=%7B%7D&skipEXIF=%7B%7D&storeAnalysisPicture=%7B%7D&storeFacePictures=%7B%7D&storePicture=%7B%7D&storeResult=%7B%7D&waitForPictureUpload=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "picture",
              "value": "{}",
              "disabled": false,
              "description": "The multipart/form-data version of the image, in case a direct upload is used"
            }
          ]
        },
        "description": "Perform detection on a given picture or picture URL"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cc20e977-0f29-4604-a697-bb47ce9c5515"
        }
      ]
    },
    {
      "id": "d2939827-242f-47ff-8ebb-3331c0ab992f",
      "name": "retriveLatestUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/analysis/listLatest?accessKey=%7B%7D&count=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Retrieve the last *count* operations per current account"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "90e259c5-6321-476d-b126-671d6c825400"
        }
      ]
    },
    {
      "id": "282e027d-ea3a-496f-bcd4-5702129d2049",
      "name": "performRecognitionUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/analysis/recognition?accessKey=%7B%7D&algorithmVersion=%7B%7D&attributeFilters=%7B%7D&collectionId=%7B%7D&filters=%7B%7D&labels=%7B%7D&options=%7B%7D&pictureURL=%7B%7D&secretKey=%7B%7D&skipEXIF rotation processing=%7B%7D&storeAnalysisPicture=%7B%7D&storeFacePictures=%7B%7D&storePicture=%7B%7D&storeResult=%7B%7D&waitForPictureUpload=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "picture",
              "value": "{}",
              "disabled": false,
              "description": "The picture itself"
            }
          ]
        },
        "description": "Perform labeled recognition on a given picture or picture URL"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "57ed942f-2a66-4545-8711-2338644b5baf"
        }
      ]
    },
    {
      "id": "4d87ffe8-eb1e-4e2f-bf0b-16a7a855a376",
      "name": "retrieveAnalysisUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/analysis/retrieve?accessKey=%7B%7D&analysisId=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Retrieve a complete analysis object including both detection and recognition information"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "989fd7a7-d2a0-4e06-ae72-2e124c8bda77"
        }
      ]
    },
    {
      "id": "c646efbe-8f13-4125-9953-4e61c1f202f4",
      "name": "counterUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/analytics/counting?accessKey=%7B%7D&collectionIds=%7B%7D&endDateTime=%7B%7D&maxBatchIterations=%7B%7D&maxIterations=%7B%7D&mergingStep=%7B%7D&minNeighborsMergedPerIteration=%7B%7D&secretKey=%7B%7D&shuffling=%7B%7D&startDateTime=%7B%7D&streamIds=%7B%7D&visitDuration=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count individuals in streams or collections"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "36dec480-025e-472d-bf99-22a9530eee31"
        }
      ]
    },
    {
      "id": "ee224816-b78f-45d4-819d-0bf793ca7943",
      "name": "presenceTimeseriesUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/analytics/presence/timeseries?accessKey=%7B%7D&attributes=%7B%7D&endDateTime=%7B%7D&secretKey=%7B%7D&startDateTime=%7B%7D&step=%7B%7D&streamIds=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Show audience (based on number of occurrences of each person) breakdown per declared attribute (age, gender)."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "057d0f17-7444-4aa0-8718-e733cf4564a2"
        }
      ]
    },
    {
      "id": "b2f086f2-a7a4-4414-b965-46f8277fcb26",
      "name": "presenceTotalUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/analytics/presence/total?accessKey=%7B%7D&attributes=%7B%7D&endDateTime=%7B%7D&secretKey=%7B%7D&startDateTime=%7B%7D&streamIds=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Show presence (based on number of occurences of each face) breakdown per declared attribute (age, gender)"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2bf49601-a82e-4555-b5a7-7b9687efa3a6"
        }
      ]
    },
    {
      "id": "be9fad19-4aa7-4199-adca-20d7d6c01ce4",
      "name": "getClassiferFullUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/classifier/svm?accessKey=%7B%7D&id=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get classifier full"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "b1bb2bee-94fd-46b0-b718-07602fe8319d"
        }
      ]
    },
    {
      "id": "5258b356-fbed-4235-aab7-b500fbd91fba",
      "name": "addSVMClassifierUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/classifier/svm?accessKey=%7B%7D&cacheSizeParameter=%7B%7D&classificationAttributeName=%7B%7D&collectionIds=%7B%7D&considerViewPoints=%7B%7D&cParameter=%7B%7D&epsParameter=%7B%7D&gammaParameter=%7B%7D&kernelTypeParameter=%7B%7D&name=%7B%7D&nuParameter=%7B%7D&preprocessor=%7B%7D&probabilityParameter=%7B%7D&secretKey=%7B%7D&seed=%7B%7D&svmTypeParameter=%7B%7D&trainingRatio=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Create new SVM classifier with given name"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "8aa758be-3d3c-4fa7-8e2e-a8618c8792d9"
        }
      ]
    },
    {
      "id": "57458c0f-172b-4754-98b0-d62d6fc2a933",
      "name": "removeClassiferUsingDELETE",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/classifier/svm?accessKey=%7B%7D&id=%7B%7D&secretKey=%7B%7D",
        "method": "DELETE",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Delete existing classifier"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "adde96ee-7df2-4e66-931d-85cd30ba0cfb"
        }
      ]
    },
    {
      "id": "53435615-190d-4add-9693-0f99b7008422",
      "name": "getClassiferStatusUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/classifier/svm/status?accessKey=%7B%7D&id=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get classifer status"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "9ce7569a-92b2-47fd-b150-e0ddc74d86fa"
        }
      ]
    },
    {
      "id": "7eeed856-9a38-4a98-bd41-ce10847b591a",
      "name": "getAllCollectionsUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/collection/?accessKey=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Retrieve all collections"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e82a1be7-55d4-4082-939c-71fe425f697d"
        }
      ]
    },
    {
      "id": "8531d508-a561-40f0-9424-abca0ca76f2d",
      "name": "addCollectionUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/collection/",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "accessKey",
              "value": "{}",
              "disabled": false,
              "description": "The accessKey provided by VisageCloud"
            },
            {
              "key": "evictable",
              "value": "{}",
              "disabled": false,
              "description": "Defined whether the collection can be evicted"
            },
            {
              "key": "name",
              "value": "{}",
              "disabled": false,
              "description": "The name of the collection that will be created"
            },
            {
              "key": "preload",
              "value": "{}",
              "disabled": false,
              "description": "Defined whether to preload collection"
            },
            {
              "key": "purposes",
              "value": "{}",
              "disabled": false,
              "description": "The newly declared purposes of the collection"
            },
            {
              "key": "secretKey",
              "value": "{}",
              "disabled": false,
              "description": "The secretKey provided by VisageCloud"
            }
          ]
        },
        "description": "Create new empty collection with given name"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "80752a08-19f2-4d28-9b02-e4551399f53c"
        }
      ]
    },
    {
      "id": "068caa30-4140-4e04-b9db-99932b718d44",
      "name": "getAllCollections2UsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/collection/all?accessKey=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Retrieve all collections"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "59d8bc78-c99c-4a0d-9cf2-c487f46d8b47"
        }
      ]
    },
    {
      "id": "b8ff3243-2583-41c9-8d62-74d90ac20f1e",
      "name": "getCollection2UsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/collection/collection?accessKey=%7B%7D&collectionId=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Retrieve existing collection content"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2e514320-ebae-47ba-bb28-e199cd456991"
        }
      ]
    },
    {
      "id": "56331e57-607b-4021-b8d4-db6b39a34ea6",
      "name": "addCollection2UsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/collection/collection?accessKey=%7B%7D&collectionName=%7B%7D&evictable=%7B%7D&preload=%7B%7D&purposes=%7B%7D&secretKey=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Create new empty collection with given name"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "5b8709ab-8d57-4693-870f-fbbe1da8a602"
        }
      ]
    },
    {
      "id": "9593dbb7-e437-42bd-811f-fe845d20401a",
      "name": "deleteCollection2UsingDELETE",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/collection/collection?accessKey=%7B%7D&collectionId=%7B%7D&secretKey=%7B%7D",
        "method": "DELETE",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Delete existing collection with associated profiles and faces."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d524d51d-cd3e-4c4b-80b3-caec3c51c61a"
        }
      ]
    },
    {
      "id": "810a94da-aac7-4c3e-b3a5-9554906c02ae",
      "name": "exportCSVUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/collection/export/csv?accessKey=%7B%7D&collectionId=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Retrieve collection content for data analysis."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "c679545a-dd39-4ef6-a52c-b1a2d5c9f704"
        }
      ]
    },
    {
      "id": "61420793-4d68-4fa8-a2d6-e9d23d14d5db",
      "name": "repurposeCollectionUsingPUT",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/collection/purpose?accessKey=%7B%7D&collectionId=%7B%7D&purposes=%7B%7D&secretKey=%7B%7D",
        "method": "PUT",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Change purpose of existing collection"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "27eb40ef-6e1f-4ffb-9b34-01aefd6fcb3d"
        }
      ]
    },
    {
      "id": "7f25b049-f7d5-41fd-a744-1a81d238d4e8",
      "name": "getCollectionUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/collection/:id"
          ],
          "query": [
            {
              "key": "accessKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "secretKey",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "id",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Retrieve existing collection content"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "6eeb88de-9af1-416e-a4f4-9323241a8409"
        }
      ]
    },
    {
      "id": "84779642-b516-49f4-8047-c3c6e747d377",
      "name": "updateCollection2UsingPOST",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/collection/:id"
          ],
          "query": [
            {
              "key": "accessKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "name",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "purposes",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "secretKey",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "id",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Update an existing collection with a given id"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2902fa1d-8aa3-4ab8-96f2-25dc647ec877"
        }
      ]
    },
    {
      "id": "7407624c-b279-428a-aa7b-4cfe022a4691",
      "name": "deleteCollectionUsingDELETE",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/collection/:id"
          ],
          "query": [
            {
              "key": "accessKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "secretKey",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "id",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "DELETE",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Delete existing collection with associated profiles and faces."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "0145f0e1-4bb4-4436-a13e-be7d36ca1abd"
        }
      ]
    },
    {
      "id": "b3048edd-866c-43d6-9bbf-ca071b13a04e",
      "name": "updateCollectionUsingPATCH",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/collection/:id"
          ],
          "query": [
            {
              "key": "accessKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "name",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "purposes",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "secretKey",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "id",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "PATCH",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Update an existing collection with a given id"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "7b238eb4-1011-4c42-ae40-9b892e86a3b3"
        }
      ]
    },
    {
      "id": "e60df50c-88ce-490f-8d7f-25e9cd0422b6",
      "name": "getAllCollectionProfilesUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/collection/:id/profile"
          ],
          "query": [
            {
              "key": "accessKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "secretKey",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "id",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Gets all the profiles associated to a collection"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cbed59a5-2803-42c4-8aa1-affaade3524d"
        }
      ]
    },
    {
      "id": "ec6ef98a-950b-4cfd-aed6-cb098f39a0da",
      "name": "getClassificationAttributesFromProfileUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/classificationAttributes?accessKey=%7B%7D&collectionId=%7B%7D&profileId=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Gets classification attributes from a profile"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "ec6cbf22-f5d9-4cdc-9188-c854aade64a6"
        }
      ]
    },
    {
      "id": "2a9b02b1-f5c9-4095-9c89-6b1c2e404bec",
      "name": "mapClassificationAttributesToProfileUsingPUT",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/classificationAttributes?accessKey=%7B%7D&classificationAttributes=%7B%7D&collectionId=%7B%7D&profileId=%7B%7D&secretKey=%7B%7D",
        "method": "PUT",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Maps classification attributes to a profile"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "c8261f39-adfd-44a4-bec4-0b561d75e7db"
        }
      ]
    },
    {
      "id": "281c0290-c3c3-4d75-827a-7a210c7915bb",
      "name": "removeClassificationAttributesFromProfileUsingDELETE",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/classificationAttributes?accessKey=%7B%7D&collectionId=%7B%7D&profileId=%7B%7D&secretKey=%7B%7D",
        "method": "DELETE",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Removes classification attributes from a profile"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "7e5770e5-f977-4463-93ef-5be9f798e57c"
        }
      ]
    },
    {
      "id": "5f2b29f2-3b09-4ea9-9ff7-c86d3c83d016",
      "name": "getProfileEnrollmentStatusUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/enrollmentStatus?accessKey=%7B%7D&collectionId=%7B%7D&profileId=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Gets the enrollment status of a profile: information on whether it is suitable for authentication."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "494aa889-b987-4f40-bfb8-ebe4c521c503"
        }
      ]
    },
    {
      "id": "00591532-7cb6-4a94-a8ae-cfa2a0293b4e",
      "name": "getFacesFromProfileUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/map?accessKey=%7B%7D&collectionId=%7B%7D&profileId=%7B%7D&secretKey=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Gets all the faceHashes associated to a profile"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "383e0348-d896-44ac-93ec-72431cc96164"
        }
      ]
    },
    {
      "id": "c1c1eb38-dfeb-4fdf-9413-970bafb75763",
      "name": "mapFacesToProfileUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/map?accessKey=%7B%7D&collectionId=%7B%7D&faceHash=%7B%7D&faceHashes=%7B%7D&profileId=%7B%7D&secretKey=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Adds (maps) a list of faces, identified by faceHashes, to a profile, identified by profileId"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cf417eb3-7b7a-408a-9dce-55c33e01922b"
        }
      ]
    },
    {
      "id": "bffa2b73-bac7-4aa1-8255-e5949e2a971c",
      "name": "removeFacesFromProfileUsingDELETE",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/map?accessKey=%7B%7D&collectionId=%7B%7D&faceHash=%7B%7D&faceHashes=%7B%7D&profileId=%7B%7D&secretKey=%7B%7D",
        "method": "DELETE",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Removes (unmaps) a list of faces, identified by faceHashes, from a profile, identified by profileId"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "70bca863-63cc-45b8-9a32-cb481f531380"
        }
      ]
    },
    {
      "id": "5950f487-e0cf-4c5d-8d25-e4a9e9e4c717",
      "name": "addProfileUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/profile?accessKey=%7B%7D&classificationAttributes=%7B%7D&collectionId=%7B%7D&details=%7B%7D&externalId=%7B%7D&labels=%7B%7D&screenName=%7B%7D&secretKey=%7B%7D",
        "method": "POST",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Creates a new profile with no faces associated to it (empty profile)"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "a8a7078b-0066-49d0-8122-0939a3f5fa75"
        }
      ]
    },
    {
      "id": "5317c228-e603-4548-991e-f8407bfe0915",
      "name": "deleteProfile2UsingDELETE",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/profile/profile?accessKey=%7B%7D&collectionId=%7B%7D&profileId=%7B%7D&secretKey=%7B%7D",
        "method": "DELETE",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Deletes a profile and unmaps all its faces"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "39398e98-2a0d-482d-9946-2a85535d25fb"
        }
      ]
    },
    {
      "id": "c8e96441-3a71-4b8e-95ee-5d5c44cbe300",
      "name": "getProfileUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/profile/:id"
          ],
          "query": [
            {
              "key": "accessKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "collectionId",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "secretKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "withFaces",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "id",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Retrieves a profile"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "8726e029-187d-4365-8068-ea6443c8350c"
        }
      ]
    },
    {
      "id": "77e1ed28-75d6-4628-bf02-2888dacb5177",
      "name": "deleteProfileUsingDELETE",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/profile/:id"
          ],
          "query": [
            {
              "key": "accessKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "collectionId",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "secretKey",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "id",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "DELETE",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Deletes a profile and unmaps all its faces"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "b8dda5b5-bbe7-46e0-8844-00caed2adfda"
        }
      ]
    }
  ]
}