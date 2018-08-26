{
  "info": {
    "name": "Visage Cloud Create new empty collection with given name",
    "_postman_id": "22f4d316-e348-4e89-81f5-4f8483fa895f",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "70f5d8b8-11a5-4712-9f1a-0689f875fa50",
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
          "id": "b9209f36-2365-4b38-8526-a632b1bacf92"
        }
      ]
    },
    {
      "id": "c62d6ccb-3b60-4368-9664-17162607f626",
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
          "id": "cdd960c9-b478-4dd8-9cac-4cb69d13e3b6"
        }
      ]
    },
    {
      "id": "4f087a0a-11b6-4c27-aa2e-b1d883aca541",
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
          "id": "b0d79842-afc4-4c0e-aefc-bf39357b638c"
        }
      ]
    },
    {
      "id": "1f4ff369-0a9d-4f90-8732-035c7b1b59a9",
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
          "id": "d7f7ff28-d1ef-4c1b-ab56-a138988993d2"
        }
      ]
    },
    {
      "id": "0bb765e6-bd46-4886-b922-e0a96ba41ab4",
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
          "id": "35775d92-bd24-4a3a-8022-708974643a2f"
        }
      ]
    },
    {
      "id": "ef8ef7ab-8590-4d72-bee6-730a66b971d3",
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
          "id": "34280c52-ecb8-4cd6-a721-249dcc9182b1"
        }
      ]
    },
    {
      "id": "3d5854f3-83a3-402a-991f-a2e15d4da18b",
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
          "id": "bf02b12f-863e-4165-ba8e-9077833970f1"
        }
      ]
    },
    {
      "id": "613c5a52-8d26-4a27-b3df-a9e268f1d191",
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
          "id": "4c3e95de-18c9-451e-8efe-c8924e6a1d25"
        }
      ]
    },
    {
      "id": "acd7227b-6b91-4a03-b10a-14d1298940d1",
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
          "id": "098b55e5-a4a2-45b3-8b3e-9dd930cb575f"
        }
      ]
    },
    {
      "id": "d90111be-e3f1-4d5b-a0f7-e5572e9002ae",
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
          "id": "ae75ea45-a112-4c0e-8138-d43ee9d88e3b"
        }
      ]
    },
    {
      "id": "c232d297-f029-44c4-847a-8a383043aec5",
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
          "id": "8d061e6b-560e-4e1b-8a89-7f949cfae9d5"
        }
      ]
    },
    {
      "id": "3e86909b-2124-4551-9bfe-0d0dfe05e44b",
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
          "id": "427d0d87-6bc8-4fb4-acc2-594f71fecb91"
        }
      ]
    },
    {
      "id": "f7f81f3f-74f3-4dd4-8e18-5547a10412e8",
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
          "id": "82279cab-d0ad-4ed2-b047-071b0d38f645"
        }
      ]
    },
    {
      "id": "0c89e674-59d6-4f39-93bf-958596baefa4",
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
          "id": "7244bfde-85c9-4f74-87d7-d015fd6504b9"
        }
      ]
    },
    {
      "id": "cebf6b6b-2a62-4e56-8e4f-0f50394aaa4d",
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
          "id": "db8d8a4d-d91a-44f4-a403-c6cd678c6145"
        }
      ]
    },
    {
      "id": "16675331-b874-4fbb-84b5-c85bcc57b0c2",
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
          "id": "f914dfa6-0259-4417-bada-284b8df9544f"
        }
      ]
    },
    {
      "id": "365871a7-139a-4b35-90a4-201ece65bad6",
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
          "id": "d3880e34-2961-4e25-85e3-9dd2183bd1d4"
        }
      ]
    },
    {
      "id": "237b64e3-5bd1-43c5-89c0-5c523f254597",
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
          "id": "3ebfe21e-9e81-4cbd-b0f2-63054e305203"
        }
      ]
    }
  ]
}