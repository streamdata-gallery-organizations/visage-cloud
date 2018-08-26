{
  "info": {
    "name": "Visage Cloud Get an existing stream with a given ID",
    "_postman_id": "4721b479-db2c-4525-91db-b6fab08f0e06",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "f58748ac-7f2f-42b7-a29c-5049dd35cf07",
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
          "id": "89b8b35e-41f6-45ac-a237-8d7de876cd28"
        }
      ]
    },
    {
      "id": "d1ce4227-50f8-4516-8d87-c582652db63f",
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
          "id": "cdc7280a-2253-419f-9460-77e59d5b18cd"
        }
      ]
    },
    {
      "id": "9a3691bf-680d-4831-8105-34c06d1553f5",
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
          "id": "e78704cc-1723-4eb0-bd3f-6b957b3ce14f"
        }
      ]
    },
    {
      "id": "618c59c2-3ff4-4834-8b18-9c294535c2a2",
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
          "id": "15d952e4-0e6e-4e82-969b-bd3e8069fb9f"
        }
      ]
    },
    {
      "id": "183d2c1b-bccc-4d5b-b976-771ae938ebd2",
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
          "id": "e2c8f8a7-cce6-4539-a2a7-18571be8b6ca"
        }
      ]
    },
    {
      "id": "cdd696ab-5383-44cd-b4c6-e6c9758ba375",
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
          "id": "4571205a-5f70-4b14-95a1-735313c02041"
        }
      ]
    },
    {
      "id": "20befc37-f921-4585-804b-58c3d9d55d28",
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
          "id": "84598a90-7cb2-4251-bb77-41d4b4889b59"
        }
      ]
    },
    {
      "id": "8e518201-2b95-44c3-82bb-6f29a60d1075",
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
          "id": "6ce5d328-387f-4004-91b4-1c4d4f5de1e0"
        }
      ]
    },
    {
      "id": "44b04649-7205-4326-8cdd-a070a621d41f",
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
          "id": "c4aaac99-3ba1-4976-b353-181068719d50"
        }
      ]
    },
    {
      "id": "1f22fccf-d368-4829-a95f-dafc310b706e",
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
          "id": "98dff4da-c267-429e-99c9-94772fdfe938"
        }
      ]
    },
    {
      "id": "d71d1e04-3fab-4acf-ad5e-b36ff29d2c1b",
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
          "id": "61860854-d916-464b-85a4-6a26cd662f64"
        }
      ]
    },
    {
      "id": "fb817368-9010-4151-92f6-6218dec3ac2d",
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
          "id": "d069afa7-315c-4980-9bfc-905b1c0c2023"
        }
      ]
    },
    {
      "id": "3f952fd3-b6f7-4b20-b650-5f5fa915b352",
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
          "id": "a4075c73-1a4c-4c46-9fda-ad375fa818a8"
        }
      ]
    },
    {
      "id": "6ecb5a58-9e2a-4624-befd-6cec3114151d",
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
          "id": "d67138da-a060-460d-a622-23d2c0b2e20c"
        }
      ]
    },
    {
      "id": "c6c96202-cd69-4b5f-9f17-082b93560228",
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
          "id": "bb1a1854-899a-43f3-bd4f-64c8054973fd"
        }
      ]
    },
    {
      "id": "1833ef2b-275b-49ef-911c-2df0b9226d33",
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
          "id": "5b3cb179-7e58-4c63-9992-defd9122c747"
        }
      ]
    },
    {
      "id": "62c1dc6b-a664-4d5b-890d-0c642677e112",
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
          "id": "beb8bab7-63d4-45a0-8475-0ef8f3373362"
        }
      ]
    },
    {
      "id": "e202ca65-42b0-4b54-bd34-746b8980ecc0",
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
          "id": "43cdd977-1d1a-42a9-aebd-675d428cc8ee"
        }
      ]
    },
    {
      "id": "f96e1587-b842-4052-b43e-ddbd02df887b",
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
          "id": "b86c7c0b-9441-4015-acdb-ff35cebc5ccf"
        }
      ]
    },
    {
      "id": "b2d11304-92dd-4dba-bd04-d43a61287700",
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
          "id": "d0bca4af-f5cb-474e-9d8c-719dfb281782"
        }
      ]
    },
    {
      "id": "1fcec9a6-32d0-45cd-affa-09b2fc268fb7",
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
          "id": "f7992013-8aaf-4fff-a5b5-f33c5a86ae06"
        }
      ]
    },
    {
      "id": "e996554e-bc27-4be6-a965-11010a4617b6",
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
          "id": "4dbc8114-1c05-407d-b78a-e525290ea626"
        }
      ]
    },
    {
      "id": "1e60e54e-fa47-4960-8790-e54d4e6b0ee1",
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
          "id": "dc1a19a6-a76b-4d05-abe5-bcf0a52136e5"
        }
      ]
    },
    {
      "id": "689111e3-874a-4cf4-a16c-447d351fd926",
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
          "id": "6718e51a-b896-4996-a780-dc87c3586e60"
        }
      ]
    },
    {
      "id": "0420e70c-ec90-4aba-b5bb-d95d49a04213",
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
          "id": "df50232f-db43-4d03-983d-115c7875cbaa"
        }
      ]
    },
    {
      "id": "12197fb0-b572-402f-862f-3d0d1a033986",
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
          "id": "48622c36-86c5-422f-a220-d90723c516d7"
        }
      ]
    },
    {
      "id": "39d7738a-322c-4962-b90d-45d871da5033",
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
          "id": "16651060-0d84-4aaf-8e8d-fd96ce95fc0c"
        }
      ]
    },
    {
      "id": "29b0a265-1d23-4d23-a129-e548a7f4e358",
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
          "id": "93d32705-2139-41a1-8248-630a13f75bef"
        }
      ]
    },
    {
      "id": "26002d57-b340-4995-b66b-a329fcaa2b29",
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
          "id": "93876f54-ea17-43ad-8aee-36037cbd145a"
        }
      ]
    },
    {
      "id": "3846eacb-cef5-4a11-8f5d-1653ddb467d6",
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
          "id": "dea1ea47-fd4b-4405-b37d-6294889d5833"
        }
      ]
    },
    {
      "id": "aeea17d3-3250-46f8-a805-408820bdac3c",
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
          "id": "8fb30f5b-10c3-4ba8-bb75-cd719f4da696"
        }
      ]
    },
    {
      "id": "26c08dd4-49c7-4eb2-94f4-4318b8f4a2b3",
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
          "id": "9d830ccf-8d48-4fa3-879b-ce88c01c522b"
        }
      ]
    },
    {
      "id": "e0bb5222-d38f-4e31-9537-158f3f76b750",
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
          "id": "7eff159f-e408-4e56-91ce-f791217d36d9"
        }
      ]
    },
    {
      "id": "f86eaa58-d319-4ea0-a7a9-5dc5033c8ab3",
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
          "id": "6876411c-f611-42bb-9184-2c6d53a5b729"
        }
      ]
    },
    {
      "id": "9289c28b-6aca-455a-bd12-16d23453fa51",
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
          "id": "4a26babd-223b-47b2-8180-dda47325ce98"
        }
      ]
    },
    {
      "id": "a9c530e9-bb0f-4884-946e-f0dd88e8055e",
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
          "id": "569b5347-20d5-4723-ae82-f3662e73e5bd"
        }
      ]
    },
    {
      "id": "03a76b7e-3ed7-4da1-9ffe-c2aa8e0861e7",
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
          "id": "feb3ffb3-1492-434d-8337-6c1687ed5df0"
        }
      ]
    },
    {
      "id": "f24aef67-9f13-4012-b010-e8c27505a7b5",
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
          "id": "3ab54dce-16ea-4403-acce-9a83fe61c4bc"
        }
      ]
    },
    {
      "id": "b77a5df3-2b5d-4885-a399-c3a604e69af2",
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
          "id": "826fd600-d70e-4c73-ae10-396a20f20785"
        }
      ]
    },
    {
      "id": "4602bb54-e2aa-472c-bd4d-956862760292",
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
          "id": "3ce60372-403f-4554-9b1b-134275b211ec"
        }
      ]
    },
    {
      "id": "cda3055a-a80b-451a-a912-cb96f13492c6",
      "name": "updateProfileUsingPATCH",
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
              "key": "classificationAttributes",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "collectionId",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "details",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "externalId",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "labels",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "screenName",
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
        "description": "Update an existing profile with a given id"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e5a604fe-804a-40eb-b0d5-25c27ea4cecd"
        }
      ]
    },
    {
      "id": "82e77327-25fb-42b0-ae76-390d0259c44a",
      "name": "streamsByAccountUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/stream/all?accessKey=%7B%7D&secretKey=%7B%7D",
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
        "description": "Show status of all streams from account"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "06a2b672-7088-48c2-a9d6-8619ff7ed7a9"
        }
      ]
    },
    {
      "id": "fef313d2-a5cf-44ef-b8b4-251e42067ba5",
      "name": "getLastNAttedanceUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/stream/attendance?accessKey=%7B%7D&count=%7B%7D&secretKey=%7B%7D&streamIds=%7B%7D",
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
        "description": "Get last N recognized individuals from stream"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fae3cc1c-fe24-4e08-a500-1b1ea6b6cb68"
        }
      ]
    },
    {
      "id": "6e4f8d6e-a475-43c3-b422-831fc9e43ba1",
      "name": "cleanupStreamUsingPATCH",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/stream/cleanup?accessKey=%7B%7D&interval=%7B%7D&secretKey=%7B%7D&streamId=%7B%7D",
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
        "description": "Cleanup frames older than specified timeframe"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "989007de-051c-4834-bcdb-97c9dfa0f0d8"
        }
      ]
    },
    {
      "id": "57f02eac-727c-4b97-8c9a-05c718bd96f0",
      "name": "getFrameImageUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/stream/frameImage?accessKey=%7B%7D&secretKey=%7B%7D&streamId=%7B%7D&timestamp=%7B%7D",
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
        "description": "Get individual frame image"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "8a06964c-1f87-471d-85c1-89b76ef45658"
        }
      ]
    },
    {
      "id": "21d2ad3f-83d3-499d-9fac-a36d9b9a99e9",
      "name": "getLastNFramesUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/stream/frames?accessKey=%7B%7D&attributeFilters=%7B%7D&collectionId=%7B%7D&count=%7B%7D&labels=%7B%7D&secretKey=%7B%7D&streamId=%7B%7D",
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
        "description": "Get last processed N frames from stream"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "f7d4de44-0ab0-4171-828b-06917a8d703c"
        }
      ]
    },
    {
      "id": "4080d463-6647-45da-b8aa-510f273d61e3",
      "name": "startStreamUsingPATCH",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/stream/start?accessKey=%7B%7D&id=%7B%7D&secretKey=%7B%7D&streamId=%7B%7D",
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
        "description": "Start existing stream"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "01c1e25d-e9f4-4b78-a765-b87f11140c2e"
        }
      ]
    },
    {
      "id": "353ca502-adfb-4c5a-880e-43100698931c",
      "name": "stopStreamUsingPATCH",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/stream/stop?accessKey=%7B%7D&id=%7B%7D&secretKey=%7B%7D&streamId=%7B%7D",
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
        "description": "Stop existing stream"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e80f913b-5235-45f5-9f5c-d09453d3f000"
        }
      ]
    },
    {
      "id": "4083895d-45b5-4f16-b9f6-95c7822e82f9",
      "name": "addStreamUsingPOST",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/stream/stream?accessKey=%7B%7D&associatedCollections=%7B%7D&attributes=%7B%7D&isActive=%7B%7D&method=%7B%7D&name=%7B%7D&password=%7B%7D&retentionTime=%7B%7D&secretKey=%7B%7D&skipFramesWithNoFaces=%7B%7D&storeAttendanceFaces=%7B%7D&storeAttendanceFrames=%7B%7D&storeOriginalFrames=%7B%7D&url=%7B%7D&username=%7B%7D",
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
        "description": "Create new stream with given name"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "74c51c7a-ea14-4eca-82e7-0afd1bc60df8"
        }
      ]
    },
    {
      "id": "89d99630-431d-4905-a015-b7bb231ee219",
      "name": "removeStreamUsingDELETE",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/stream/:id"
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
        "description": "Delete existing stream"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "54b1455e-d3b5-4687-85ce-9d6a98a07c80"
        }
      ]
    },
    {
      "id": "9825e959-c76b-4a41-ad15-4560e9d13bb8",
      "name": "getStreamUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "visagecloud.com",
          "path": [
            "rest/v1.1/stream/:streamId"
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
              "id": "streamId",
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
        "description": "Get an existing stream with a given ID"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "62319424-7abe-4e0b-b84c-98045c7dfefd"
        }
      ]
    }
  ]
}