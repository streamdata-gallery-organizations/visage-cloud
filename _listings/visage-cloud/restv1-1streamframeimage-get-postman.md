{
  "info": {
    "name": "Visage Cloud Get individual frame image",
    "_postman_id": "6aa41d5b-692e-431d-a0af-359f89800a2a",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "0ce1ebf2-a392-44b8-99b6-0ac36e9ccc50",
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
          "id": "f4d22183-0086-4147-a959-5a52659410f6"
        }
      ]
    },
    {
      "id": "12fc154c-f8fd-407a-8adf-b47df1f24886",
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
          "id": "b06feb03-1b93-4cfc-aaac-e9e0f1a8bfaf"
        }
      ]
    },
    {
      "id": "74f7e6cb-7275-48aa-93f1-db8d3b766e14",
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
          "id": "6c6ed153-8edf-47eb-84ea-82f85e014312"
        }
      ]
    },
    {
      "id": "0bd33454-d97e-41d5-833b-d58324271b73",
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
          "id": "2d90e1d7-9841-4021-be04-40fa2bd538e1"
        }
      ]
    },
    {
      "id": "87e343e8-a915-4a0e-bc6f-64342fc04796",
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
          "id": "a5be68fe-06af-4e90-a4d1-bdc554f63769"
        }
      ]
    },
    {
      "id": "9aac57f3-b824-4ee4-b3a7-eaf1cb4188e9",
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
          "id": "e41f3a63-939e-42f2-98c0-1b4534022fd4"
        }
      ]
    },
    {
      "id": "085fe78f-9e3d-478f-af79-1fa7c794eb00",
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
          "id": "0ca32f37-7aec-4184-bee7-c5b008b4ff01"
        }
      ]
    },
    {
      "id": "94434370-1cc4-4e31-a64a-3b31b3d376bf",
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
          "id": "6eaf64a9-53b8-4d62-bd2b-a3b28850327d"
        }
      ]
    },
    {
      "id": "eb1f88a6-3041-418a-a4bc-a1f6325f8df7",
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
          "id": "6c9ae60c-db08-44dc-b967-47f6c61be4be"
        }
      ]
    },
    {
      "id": "f7e65dc9-e714-4380-9416-1bb8fb67845f",
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
          "id": "48c2c7a5-ed69-419e-9f5a-a5e2e51763d7"
        }
      ]
    },
    {
      "id": "be932a1b-203c-4ff5-8208-0dca8863939e",
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
          "id": "6cfdaa9f-956f-4d13-9c21-040e6dace28d"
        }
      ]
    },
    {
      "id": "ca8e9cb6-8442-4194-b387-7597da65f8c0",
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
          "id": "707a69bc-005c-4dde-a9bf-e629a1a626b8"
        }
      ]
    },
    {
      "id": "1778943f-4d90-4707-93b4-2b066bac3922",
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
          "id": "d5c46863-eb06-4f25-9229-c41363a926b4"
        }
      ]
    },
    {
      "id": "b96f5e85-9b13-4e92-bfbb-bc6e5ea14f6d",
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
          "id": "bbec5446-22d7-44f7-979e-17bd1aa2a8a2"
        }
      ]
    },
    {
      "id": "b853ec68-242c-45b7-b3b2-024f29a05649",
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
          "id": "0f68663f-8e45-4232-ad11-00c98d57105c"
        }
      ]
    },
    {
      "id": "e9dd4820-ca4d-4300-8267-1898fd2da824",
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
          "id": "465f9081-03d7-4d3e-8297-39b8f9f3d019"
        }
      ]
    },
    {
      "id": "ab7bb680-09c6-432a-bf83-3bb58bad0b7d",
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
          "id": "c4c0b889-0f8b-4884-b98e-616240db0bb2"
        }
      ]
    },
    {
      "id": "b49a5e77-c9c6-4fdc-be2a-af26e132da8a",
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
          "id": "6df32c2a-e943-41aa-8166-c5d79a512346"
        }
      ]
    },
    {
      "id": "c62210a5-3a90-4697-9092-6d41a0cbaa3b",
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
          "id": "121a3b6d-82f2-4c42-9c4d-2afc4ecf67c1"
        }
      ]
    },
    {
      "id": "6b9949f4-5b17-4c81-82bf-049946f43ca1",
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
          "id": "aa17486f-5ca5-4ec3-8281-0435ee41a633"
        }
      ]
    },
    {
      "id": "5b2ee747-9a5f-46d4-9cbc-b9245f9ea5d5",
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
          "id": "7165d53f-5c5f-49df-a8cb-a173ea02add4"
        }
      ]
    },
    {
      "id": "4cdb0897-35a9-4b65-b196-c603c1075cb6",
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
          "id": "144db50b-3a0d-4b09-8fb1-a741abfdbf8b"
        }
      ]
    },
    {
      "id": "e3501dba-3bbb-4270-9664-433a227ebe7c",
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
          "id": "993b375b-08d2-4230-8095-b0f874229a6f"
        }
      ]
    },
    {
      "id": "643b546e-41e4-40cc-b311-b1d6b25e604f",
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
          "id": "c3bdcef3-e8af-44da-b730-b5e19d6dc4b5"
        }
      ]
    },
    {
      "id": "6b902409-9320-4b38-8cc4-cf7fa4d130c3",
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
          "id": "d0814837-d3f4-4b7b-904a-7448a9cd1edb"
        }
      ]
    },
    {
      "id": "ebec5b72-c5b9-41d0-9914-680578cc2dea",
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
          "id": "d741352c-8526-464a-b36f-a7dada03b246"
        }
      ]
    },
    {
      "id": "119bc64c-29dd-4db2-984b-25438a034ff5",
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
          "id": "cd64f747-47a4-4c0a-a0fd-b3d59fe794ea"
        }
      ]
    },
    {
      "id": "60d6e434-9755-4902-a670-f4653aa8ac7f",
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
          "id": "4971d32c-d970-4315-ab11-3fd885ab2f30"
        }
      ]
    },
    {
      "id": "7af17bfd-1fcd-452e-a702-790e0c325caa",
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
          "id": "544aab79-6204-4a1f-a76e-a2d91ef7ffc4"
        }
      ]
    },
    {
      "id": "badf92c0-386d-45c6-bc5a-f4564ad0592b",
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
          "id": "f2643a35-b185-4c18-9120-0464ee9cb126"
        }
      ]
    },
    {
      "id": "457e59e8-5edc-4008-a73a-6b6a2fa572d6",
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
          "id": "c40a0dc6-0fd6-4f70-b042-7fd8247a171f"
        }
      ]
    },
    {
      "id": "7da92f54-0fd7-4165-9d76-12fd1caa244d",
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
          "id": "29eaf503-d1ae-489f-97d8-a0d1d6dfd121"
        }
      ]
    },
    {
      "id": "f6da4848-e9ae-4e5a-808f-c280f46a3b91",
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
          "id": "242e6b37-51b6-48d9-bb80-215a4b765038"
        }
      ]
    },
    {
      "id": "d99f3528-e342-4853-82e3-bf312042bf6d",
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
          "id": "a918b165-1d88-4dca-98ac-c4beecacf703"
        }
      ]
    },
    {
      "id": "64b25286-fbe7-4d38-894e-215c36460109",
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
          "id": "b846bc28-c37c-4340-9580-cb23481062b7"
        }
      ]
    },
    {
      "id": "c5fdf3b1-4b5e-48dc-9ce9-5bd672492edb",
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
          "id": "1868e301-5b2c-41f8-82c5-cbb1e35772df"
        }
      ]
    },
    {
      "id": "ac80ce26-d17c-44eb-8847-d679402b302b",
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
          "id": "1101ec65-7c2e-4911-a0ae-439ba6a17f4b"
        }
      ]
    },
    {
      "id": "c525e89c-d345-4c06-bacc-71770980dbf7",
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
          "id": "1d089cc9-945c-43ce-9911-0eb9fc8e054b"
        }
      ]
    },
    {
      "id": "d4c5934e-f1d7-4364-83eb-cc8074cc4625",
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
          "id": "29cc4228-98fc-4f0d-bcee-41bf73726cc9"
        }
      ]
    },
    {
      "id": "f5f7ec4a-87f4-4a37-aafc-33ff9b36decc",
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
          "id": "f367f410-a0f8-4bb6-b30c-0fb47877ede8"
        }
      ]
    },
    {
      "id": "48954798-8714-4e6f-be90-01a4563bdac9",
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
          "id": "f23f23e4-4863-4a37-aa9c-2a4161c464c2"
        }
      ]
    },
    {
      "id": "de691ab5-9e74-4c3e-a48a-d024b6c02240",
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
          "id": "9561df36-be3e-48ad-a958-0e569d31b051"
        }
      ]
    },
    {
      "id": "38a32de1-9eb8-46cd-ad86-44ad9739709b",
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
          "id": "c4003e3e-5d14-405a-ae6c-8885b2c31f80"
        }
      ]
    },
    {
      "id": "8d37e9ba-e6a4-4fa7-8cdb-338b37a7174e",
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
          "id": "01abc2b4-37b6-4465-b224-cfa9679b3033"
        }
      ]
    },
    {
      "id": "a9773e9d-3094-49a7-a24a-47807f99cb7f",
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
          "id": "4642e8ba-8e34-4616-8fec-b37e414577c5"
        }
      ]
    }
  ]
}