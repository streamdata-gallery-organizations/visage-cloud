{
  "info": {
    "name": "Visage Cloud Removes (unmaps) a list of faces, identified by faceHashes, from a profile, identified by profileId",
    "_postman_id": "9bd1cdf7-05a5-4dc4-8776-7b0860b711ba",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "612b2026-44e3-47a5-b05a-6ad62d966765",
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
          "id": "aa462d69-e42e-444b-8222-2a303599b6f2"
        }
      ]
    },
    {
      "id": "b60be5e9-e990-4421-8f8e-5a80c6673c7f",
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
          "id": "29b28da2-f6af-42a8-b09b-e8bbc711fa53"
        }
      ]
    },
    {
      "id": "ad5b61b9-f6fb-4337-9e3c-969eefa1f601",
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
          "id": "182d79fd-2269-4dd8-b944-b582bf750dd1"
        }
      ]
    },
    {
      "id": "0f6e627e-e034-4678-97ed-eb9e3d7b32ca",
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
          "id": "6eff9ff6-bd25-40c1-b479-947eba975a4a"
        }
      ]
    },
    {
      "id": "fabe3363-e52f-478b-838d-4e0033ff32ff",
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
          "id": "3b1f996b-2a56-4cde-b3d1-7ae182b0e2f4"
        }
      ]
    },
    {
      "id": "dcf7fea4-1cea-47b3-bb3d-6744b100b840",
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
          "id": "7865bf46-6ecc-4b65-a80f-545923fba805"
        }
      ]
    },
    {
      "id": "22166359-6749-46ae-9723-c3f4d7e80aa2",
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
          "id": "00ab0682-eb90-41be-a87d-54b5fe6f8853"
        }
      ]
    },
    {
      "id": "4e833c2f-c10b-4731-810d-8f1c1d0b1e38",
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
          "id": "8a6fb7e3-d6b2-4d74-9a82-42ee5c82fabe"
        }
      ]
    },
    {
      "id": "70948780-4cf7-4363-8727-548841772eae",
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
          "id": "4a9542b4-7cd6-420a-8957-7b739987ab14"
        }
      ]
    },
    {
      "id": "2a1ccffa-f3c0-45ed-b0bb-1492f5e29da6",
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
          "id": "fb621a94-b9e2-40cc-a6b4-0b2f30d3f9ce"
        }
      ]
    },
    {
      "id": "4e51bc95-e26c-4d93-8935-382121f8ceb8",
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
          "id": "46c8a760-ca58-4abe-b951-ccaff7210065"
        }
      ]
    },
    {
      "id": "9ba9b335-5b96-4b90-a39e-b28699caf37e",
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
          "id": "b81795cd-2918-4ff1-ba41-238ff36cda9a"
        }
      ]
    },
    {
      "id": "517c8246-a0fe-4a70-93ac-6f5761222ccd",
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
          "id": "b4faf0ed-aa41-4323-9145-dc86bacaa910"
        }
      ]
    },
    {
      "id": "c44d51c9-3409-4a8a-9eba-85d7fd239848",
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
          "id": "8b8bf835-7dbe-4368-b4dd-9341eb515669"
        }
      ]
    },
    {
      "id": "16998147-1751-499b-89e7-a355095d86b7",
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
          "id": "90a4cd7f-be32-4ab5-a85f-a03dd090c350"
        }
      ]
    },
    {
      "id": "056db88b-a79e-45c6-b3b9-a2893764d74c",
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
          "id": "c165c7e6-ec6f-4ec6-aa4c-f3cf86eb1394"
        }
      ]
    },
    {
      "id": "2bd61363-7b11-4c73-87df-ba335e5badbf",
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
          "id": "7509524f-f22b-43f3-b9ff-73de5ac95a19"
        }
      ]
    },
    {
      "id": "da69f210-4c36-458c-92ad-9b4b6512bb86",
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
          "id": "66571d4c-d5dd-4b4d-95b2-8ffe8d91aa14"
        }
      ]
    },
    {
      "id": "0e57682d-ccac-48ac-8155-15cb77ce3eea",
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
          "id": "607f3eba-6e69-419c-b679-b37b903bc798"
        }
      ]
    },
    {
      "id": "1f185a16-a8c8-4d60-bc8c-edcebeebdbee",
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
          "id": "7bf5cb3c-94bd-4cf3-88f8-28f2dfa38fd6"
        }
      ]
    },
    {
      "id": "f9099d1c-3d69-41fe-8369-c3210e347e0b",
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
          "id": "55ef337e-b2eb-4918-9e5a-ef58402cc095"
        }
      ]
    },
    {
      "id": "ede354a5-daed-4078-92dc-ed238317efbf",
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
          "id": "b19acf83-75ae-4716-87c4-795f61b1d1e5"
        }
      ]
    },
    {
      "id": "a4187b92-e335-4fe0-afd8-38d863bf6a8f",
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
          "id": "6207fc4f-b520-495a-aa5f-680431b2d256"
        }
      ]
    },
    {
      "id": "cbba1ee7-1c1a-425b-945e-074974425630",
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
          "id": "98303ee4-8d8f-4bcd-9330-70f06780eacc"
        }
      ]
    },
    {
      "id": "2666d497-e2fb-46db-9f96-95b063bcb67e",
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
          "id": "447d3700-13ab-4b04-b9e6-69bde5d1933c"
        }
      ]
    },
    {
      "id": "a0ae28c4-b2a0-4cec-9492-d43528e7ecae",
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
          "id": "a7fe2c58-5d83-451d-bb03-8d758b93d053"
        }
      ]
    },
    {
      "id": "485c2e29-573e-46ff-9aa5-8cb53e4e538d",
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
          "id": "44aefd2c-b26b-47d2-bd6e-80e60edb6b65"
        }
      ]
    },
    {
      "id": "d524acec-abf1-4df1-9cb7-3610155c90cb",
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
          "id": "0ba518d3-168c-4369-a77c-ed40e2a201ca"
        }
      ]
    },
    {
      "id": "8e95487f-97d2-4da7-9b31-601aa7535956",
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
          "id": "0e2e5643-4f30-4c20-ba5c-2690ed93d4d5"
        }
      ]
    },
    {
      "id": "5e70cea2-2800-4039-8f2e-1346d1c9cb09",
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
          "id": "a63b59b5-391c-4a85-bbe1-fe2181c0ba0e"
        }
      ]
    },
    {
      "id": "b8b0ff85-5d38-4fff-ba47-1f64af231a98",
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
          "id": "070a9c50-4900-4bd7-9798-59fec1dbfc98"
        }
      ]
    },
    {
      "id": "be8ea8e6-2530-4cc6-8069-854ac18639d8",
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
          "id": "39c70d09-5873-4d4c-b74a-fabe731edf1e"
        }
      ]
    },
    {
      "id": "89bc9406-f8fd-4b76-8ed1-f0c0963b6b0b",
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
          "id": "bcc32d87-64b3-422f-9e1e-f8c722b0319b"
        }
      ]
    },
    {
      "id": "9ef57672-21eb-4565-83c2-587122d57deb",
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
          "id": "f000a19d-f77d-4581-b918-1879f2f85715"
        }
      ]
    }
  ]
}