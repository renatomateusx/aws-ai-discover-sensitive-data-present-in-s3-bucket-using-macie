[export-2024-03-11T19_52_51Z.json](https://github.com/renatomateusx/aws-ai-discover-sensitive-data-present-in-s3-bucket-using-macie/files/14563949/export-2024-03-11T19_52_51Z.json)#  Project made to improve skills with focus on Machine Learning using macie for detecting sensitive data inside S3 Buckets

# Task Details

* 1 - Sign in to AWS Management Console.
* 2 - Enable Macie for the account.
* 3 - Create a Macie job.
* 4 - Macie job run and findings.
* 5 - Validation of the lab.

# Project Arch
![macie_project_arch](https://github.com/renatomateusx/aws-ai-discover-sensitive-data-present-in-s3-bucket-using-macie/assets/4579323/d4d25c5f-1d90-4a16-90bd-ac64a095cdb3)

# JSON Result Preview


[Uploading export-2024-03-11T19_52_51[
  {
    "accountId": "843257763552",
    "archived": false,
    "category": "CLASSIFICATION",
    "classificationDetails": {
      "detailedResultsLocation": "s3://[export-config-not-set]/AWSLogs/843257763552/Macie/us-east-1/8df4fca1eccfdae45d8b936a21f1882d/843257763552/fe48af52-aad0-3665-8ebb-87432a08ee6f.jsonl.gz",
      "jobArn": "arn:aws:macie2:us-east-1:843257763552:classification-job/8df4fca1eccfdae45d8b936a21f1882d",
      "jobId": "8df4fca1eccfdae45d8b936a21f1882d",
      "originType": "SENSITIVE_DATA_DISCOVERY_JOB",
      "result": {
        "additionalOccurrences": false,
        "customDataIdentifiers": {
          "detections": [
            {
              "arn": "0e8eb8a1-1a3a-49ad-992f-0ab825642859",
              "count": 3,
              "name": "Whiz",
              "occurrences": {
                "cells": [
                  {
                    "cellReference": null,
                    "column": 1,
                    "columnName": "EmpID",
                    "row": 2
                  },
                  {
                    "cellReference": null,
                    "column": 1,
                    "columnName": "EmpID",
                    "row": 4
                  },
                  {
                    "cellReference": null,
                    "column": 1,
                    "columnName": "EmpID",
                    "row": 5
                  }
                ]
              }
            }
          ],
          "totalCount": 3
        },
        "mimeType": "text/csv",
        "sensitiveData": [],
        "sizeClassified": 80,
        "status": {
          "code": "COMPLETE",
          "reason": null
        }
      }
    },
    "count": 1,
    "createdAt": "2024-03-11T19:46:53.031Z",
    "description": "The S3 object contains text that matches the criteria of one or more custom data identifiers. The object might contain multiple types of sensitive data.",
    "id": "ba3c75616234b8a67797b8000371aaba",
    "partition": "aws",
    "region": "us-east-1",
    "resourcesAffected": {
      "s3Bucket": {
        "allowsUnencryptedObjectUploads": "TRUE",
        "arn": "arn:aws:s3:::whizlabs.183836.81670451",
        "createdAt": "2024-03-11T19:37:03.000Z",
        "defaultServerSideEncryption": {
          "encryptionType": "AES256",
          "kmsMasterKeyId": null
        },
        "name": "whizlabs.183836.81670451",
        "owner": {
          "displayName": "labsorganization93",
          "id": "9ff21031f6ad6d32437ce9668c459d513416439f85260bb5cece1acbaacdfb7e"
        },
        "publicAccess": {
          "effectivePermission": "PUBLIC",
          "permissionConfiguration": {
            "accountLevelPermissions": {
              "blockPublicAccess": {
                "blockPublicAcls": false,
                "blockPublicPolicy": false,
                "ignorePublicAcls": false,
                "restrictPublicBuckets": false
              }
            },
            "bucketLevelPermissions": {
              "accessControlList": {
                "allowsPublicReadAccess": false,
                "allowsPublicWriteAccess": false
              },
              "blockPublicAccess": {
                "blockPublicAcls": false,
                "blockPublicPolicy": false,
                "ignorePublicAcls": false,
                "restrictPublicBuckets": false
              },
              "bucketPolicy": {
                "allowsPublicReadAccess": true,
                "allowsPublicWriteAccess": true
              }
            }
          }
        },
        "tags": []
      },
      "s3Object": {
        "bucketArn": "arn:aws:s3:::whizlabs.183836.81670451",
        "eTag": "07b21b45c9ed4a3fabf8173be102d9c2",
        "extension": "csv",
        "key": "sample_data.csv",
        "lastModified": "2024-03-11T19:37:04.000Z",
        "path": "whizlabs.183836.81670451/sample_data.csv",
        "publicAccess": null,
        "serverSideEncryption": {
          "encryptionType": "AES256",
          "kmsMasterKeyId": null
        },
        "size": 80,
        "storageClass": "STANDARD",
        "tags": [],
        "versionId": ""
      }
    },
    "sample": false,
    "schemaVersion": "1.0",
    "severity": {
      "description": "Medium",
      "score": 2
    },
    "title": "The S3 object contains text that matches custom data identifier criteria",
    "type": "SensitiveData:S3Object/CustomIdentifier",
    "updatedAt": "2024-03-11T19:46:53.031Z"
  }
]Z.json…]()
