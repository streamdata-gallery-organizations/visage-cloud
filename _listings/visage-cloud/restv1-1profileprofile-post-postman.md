{
  "info": {
    "name": "Visage Cloud Creates a new profile with no faces associated to it (empty profile)",
    "_postman_id": "e9f72777-9b66-41e0-91e6-194e1092c178",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "6de88f1c-f8d6-4ac5-b90c-e927e77a9c0e",
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
          "id": "98a26985-3cea-4d2f-b1f2-6521ae96b17e"
        }
      ]
    },
    {
      "id": "d6ba11fb-60c1-481e-ad39-ef4e8ff2efc4",
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
          "id": "164916d5-dbc4-4d10-93cf-3750f8908e2d"
        }
      ]
    },
    {
      "id": "c6682e68-f7fe-4829-b816-72bfa637ee1c",
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
          "id": "b90171a9-e296-458d-956b-7b66dc440cf6"
        }
      ]
    },
    {
      "id": "54b14c90-fbac-4b81-b71b-6a3e906bc10c",
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
          "id": "174480d3-8b39-4682-89f3-c99adb3a4d57"
        }
      ]
    },
    {
      "id": "4c4d7188-9573-4278-a8f3-9275c0384efb",
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
          "id": "925597b7-ae61-4609-86ff-a087e544f606"
        }
      ]
    },
    {
      "id": "542ba94a-dcf5-4b2b-afa3-9f59776d4350",
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
          "id": "58777b95-579b-4e0d-9d03-9a746b5cc133"
        }
      ]
    },
    {
      "id": "322156fd-0794-4c50-9ca1-0222f4ad0850",
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
          "id": "81412aaf-c6f0-425c-b81f-96f402fadc77"
        }
      ]
    },
    {
      "id": "f44d09f1-3f0c-4b7b-889c-85127057c26f",
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
          "id": "d84e1535-590c-4d06-a414-2fce6ac0d536"
        }
      ]
    },
    {
      "id": "bbb2faec-2d7a-4c05-823b-d28df769524b",
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
          "id": "c6676d7a-5e02-45e0-87ad-20e18e54e7f4"
        }
      ]
    },
    {
      "id": "004caae9-0afb-4f3b-9762-7327c020e2fb",
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
          "id": "11d192fb-ffe1-4e7b-bcca-10c157d48911"
        }
      ]
    },
    {
      "id": "f37e73c4-ed6c-40ad-95cb-796aead9932d",
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
          "id": "636721e9-2dff-40c7-9785-9ed8b2329fdc"
        }
      ]
    },
    {
      "id": "f6d4665b-0686-49f7-b482-d52594154d1b",
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
          "id": "b9d2e724-1241-4381-8d2f-b7a1482c2cd1"
        }
      ]
    },
    {
      "id": "db624edb-a02d-4fb1-8825-b1464fe637ef",
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
          "id": "2e0cc9de-ecaf-4d36-8354-3ccd9c5f2768"
        }
      ]
    },
    {
      "id": "b9e01a47-fba7-4c75-91bb-e42f0af62245",
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
          "id": "954ff775-7456-46de-9502-d27ea1fd6c28"
        }
      ]
    },
    {
      "id": "b9667fe8-bb18-437f-a032-5ac035891224",
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
          "id": "2cae5b32-3044-4a48-9561-2e17e9874392"
        }
      ]
    },
    {
      "id": "fca81d9f-b09e-43ea-8bf3-de9b914c972f",
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
          "id": "7cc7e11e-e17f-4df4-8ad2-be0f3bd9abff"
        }
      ]
    },
    {
      "id": "017ba0e1-68b2-4fb5-8d58-87e20fdde7f0",
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
          "id": "689add5f-cf4b-4351-bd79-313370e69160"
        }
      ]
    },
    {
      "id": "c63a6f41-991f-4d11-b214-5d5de722219d",
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
          "id": "80f12143-4b83-4206-8c7b-3f79dc2994c3"
        }
      ]
    },
    {
      "id": "70b49962-459e-4a60-93ac-2cd2504fce29",
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
          "id": "73f4e836-8e47-4a7d-a2ef-b747b45ea737"
        }
      ]
    },
    {
      "id": "cf0754a3-03f2-4a25-95ec-786fbc8e5969",
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
          "id": "bbb1f1fe-d291-4d96-a632-db60d583c9aa"
        }
      ]
    },
    {
      "id": "e8d6ceb2-f4e3-4d0d-8aca-7c7d71c06648",
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
          "id": "70ab7ef3-ed22-403d-aa48-7016df312ec9"
        }
      ]
    },
    {
      "id": "9c26e15e-73c0-4c3a-9292-d6522bd276ce",
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
          "id": "733718e9-740a-472b-b2da-687673e8d4a9"
        }
      ]
    },
    {
      "id": "027cd22c-81fe-44ae-91a0-dc5ca545b9ea",
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
          "id": "3acb54da-1ed4-428e-9551-6f4ad3de3d14"
        }
      ]
    },
    {
      "id": "efa0f91d-d892-4dff-b96f-1c583c708585",
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
          "id": "445b1643-79b0-4684-81b7-15ea34586927"
        }
      ]
    },
    {
      "id": "dde36d9a-3b8f-438b-ab1c-e1dd40aae6be",
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
          "id": "9a9d10b5-8adb-48cd-a40d-c2a2682e88bb"
        }
      ]
    },
    {
      "id": "b04dad4c-e0eb-44e1-9012-04bca5fe604d",
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
          "id": "6477e00d-48e4-45f9-9b98-4529a83ebac6"
        }
      ]
    },
    {
      "id": "c08b5999-3487-43c9-a25f-bcee5eef58a9",
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
          "id": "9c3d380e-bce8-40f9-8906-55030aeb30cd"
        }
      ]
    },
    {
      "id": "78a6fddb-e7fa-4ee5-8766-125f57403bcc",
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
          "id": "64237b33-a767-4f69-8366-c37f2e189d69"
        }
      ]
    },
    {
      "id": "9379c821-d185-479d-92b2-3b4c1fe88d45",
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
          "id": "4ad69f6f-9e48-42ca-aa32-26e4d807ef93"
        }
      ]
    },
    {
      "id": "c33140d9-facb-4943-9f29-a30dbcc87960",
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
          "id": "d2440233-8cf9-4be8-8d8f-19245cf91416"
        }
      ]
    },
    {
      "id": "b4a4ee30-9704-4313-af78-67266f26a8fc",
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
          "id": "9ad372d1-54b6-40f3-b804-02b3d5791abf"
        }
      ]
    },
    {
      "id": "372319d3-5f2b-47e5-bcf9-5b5d1408d262",
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
          "id": "f9915bca-decb-4f0f-8124-e72ed28b5d4a"
        }
      ]
    },
    {
      "id": "3d42e4cd-631d-43fa-876c-7405a598c6a6",
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
          "id": "0d579223-38ff-403e-84d7-6a6b5cef9b8f"
        }
      ]
    },
    {
      "id": "8ef25c10-c779-444e-9324-42c6624f9692",
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
          "id": "72095e29-14d3-48f7-afb8-2900725b80bd"
        }
      ]
    },
    {
      "id": "d51a0b29-7f9e-4bab-8cab-d13b4e553b10",
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
          "id": "33416a04-f9c2-4d84-bd93-84f1c4e643b8"
        }
      ]
    },
    {
      "id": "0f4bebd4-3c26-47ce-b10c-888c32a98139",
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
          "id": "c76990b6-c0b8-4d63-bce9-d091424cd048"
        }
      ]
    },
    {
      "id": "a953f730-b4fe-4fb2-8ef2-9247d2aa5e29",
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
          "id": "e7ed5e35-6af4-45f5-9180-65fb9843543a"
        }
      ]
    },
    {
      "id": "31f9791f-0d5e-4b02-833f-28f2ed499a60",
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
          "id": "e0da3a10-140d-4c8a-899b-be9fe81663c3"
        }
      ]
    }
  ]
}