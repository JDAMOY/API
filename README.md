## 1: Get GR detail
####   localhost:8888/tradeshift-backend/rest/external/documents/4100d1ca-4b28-4b78-90b8-9410bdf6a644
  ```javascript
  {
  "DocumentType": "ReceiptAdviceType",
  "UBLVersionID": {
    "value": "2.0"
  },
  "CustomizationID": {
    "value": "urn:tradeshift.com:ubl-2.0-customizations:2010-06"
  },
  "ProfileID": {
    "value": "urn:tradeshift.com:profile:BasicReceiptAdvice:ver1.0",
    "schemeAgencyID": "http://tradeshift.com"
  },
  "ID": {
    "value": "10086005"
  },
  "IssueDate": {
    "value": "2016-12-17"
  },
  "Note": [
    {
      "value": "Recieved by Alex M."
    }
  ],
  "OrderReference": [
    {
      "ID": {
        "value": "201400002"
      }
    }
  ],
  "DeliveryCustomerParty": {
    "Party": {
      "PartyIdentification": [
        {
          "ID": {
            "value": "9b42f49e-028d-43cc-b6fa-6e24b2a43dc9",
            "schemeID": "TS:ID"
          }
        }
      ],
      "PartyName": [
        {
          "Name": {
            "value": "[Test] - Bilfinger EMS GmbH, Cloppenburg"
          }
        }
      ],
      "PostalAddress": {
        "AddressFormatCode": {
          "value": "5",
          "listID": "UN/ECE 3477",
          "listAgencyID": "6",
          "listVersionID": "D08B"
        },
        "StreetName": {
          "value": "Hohe Tannen"
        },
        "BuildingNumber": {
          "value": "11"
        },
        "CityName": {
          "value": "Cloppenburg"
        },
        "PostalZone": {
          "value": "49661"
        },
        "Country": {
          "IdentificationCode": {
            "value": "DE"
          }
        }
      },
      "Contact": {
        "ID": {
          "value": "najier01@163.com"
        }
      }
    }
  },
  "DespatchSupplierParty": {
    "Party": {
      "EndpointID": {
        "value": "DE123456781",
        "schemeID": "DE:VAT"
      },
      "PartyIdentification": [
        {
          "ID": {
            "value": "4d2a8097-d00e-41da-8a38-71b425566c89",
            "schemeID": "TS:ID"
          }
        }
      ],
      "PartyName": [
        {
          "Name": {
            "value": "Test Supplier for BF"
          }
        }
      ],
      "PostalAddress": {
        "AddressFormatCode": {
          "value": "5",
          "listID": "UN/ECE 3477",
          "listAgencyID": "6",
          "listVersionID": "D08B"
        },
        "StreetName": {
          "value": "Langenhorner"
        },
        "BuildingNumber": {
          "value": "10"
        },
        "CityName": {
          "value": "Hamburg"
        },
        "PostalZone": {
          "value": "22419"
        },
        "Country": {
          "IdentificationCode": {
            "value": "DE"
          }
        }
      },
      "PartyTaxScheme": [
        {
          "CompanyID": {
            "value": "DE123456781",
            "schemeID": "DE:VAT"
          },
          "TaxScheme": {
            "Name": {
              "value": "VAT"
            }
          }
        }
      ],
      "Contact": {}
    }
  },
  "ReceiptLine": [
    {
      "ID": {
        "value": "1"
      },
      "Note": {
        "value": "Undamaged"
      },
      "ReceivedQuantity": {
        "value": 3,
        "unitCode": "EA"
      },
      "OrderLineReference": {
        "LineID": {
          "value": "1"
        }
      },
      "Item": [
        {
          "Description": [
            {
              "value": "我的打印机"
            }
          ],
          "Name": {
            "value": "激光打印机"
          },
          "SellersItemIdentification": {
            "ID": {
              "value": "10",
              "schemeID": "GTIN",
              "schemeAgencyID": "9"
            }
          }
        }
      ]
    },
    {
      "ID": {
        "value": "2"
      },
      "Note": {
        "value": "Undamaged"
      },
      "ReceivedQuantity": {
        "value": 1,
        "unitCode": "EA"
      },
      "OrderLineReference": {
        "LineID": {
          "value": "2"
        }
      },
      "Item": [
        {
          "Description": [
            {
              "value": "我买的打印纸"
            }
          ],
          "Name": {
            "value": "打印纸"
          },
          "SellersItemIdentification": {
            "ID": {
              "value": "20",
              "schemeID": "GTIN",
              "schemeAgencyID": "9"
            }
          }
        }
      ]
    }
  ]
}
```
## 2: Get proforma template 
####   

## 3: Get conversation history [TODO: user title user logo] 
####   localhost:8888/tradeshift-backend/rest/external/conversations/documents/a714ed57-e96a-56db-a445-7e4a85ae487f?enrich=false
```javascript
{
  "itemsPerPage": 0,
  "itemCount": 0,
  "numPages": -1,
  "pageId": -1,
  "Conversation": [
    {
      "ID": "96d7e60f-e1c5-4c7d-a997-5912aa3f0b1e",
      "ConversationId": "8a8765c5-0e09-4969-86ab-1cb4b0131315",
      "ObjectId": "0730f30e-a87f-53da-95b7-476222200047",
      "ObjectType": 10015,
      "Type": "Proforma",
      "Timestamp": "2016-12-20T17:15:13.727+08:00",
      "LastChange": "2016-12-20T17:15:13.727+08:00",
      "State": "RECEIVED",
      "History": [],
      "HistoryAvailable": false,
      "UnifiedStateCausedByOtherParty": false,
      "Received": false,
      "AllowedActions": [],
      "Initiator": {
        "CompanyAccountId": "4d2a8097-d00e-41da-8a38-71b425566c89",
        "CompanyAccountName": "중국어001公司",
        "UserId": "052504ec-fe7d-4816-833e-58af5b5af5c0",
        "UserName": "중국어001联系 001"
      },
      "PendingDocument": false,
      "Visible": false
    },
    {
      "ID": "10ec9516-130a-4a4c-95f1-8f88446544c3",
      "ConversationId": "8a8765c5-0e09-4969-86ab-1cb4b0131315",
      "ObjectId": "a714ed57-e96a-56db-a445-7e4a85ae487f",
      "ObjectType": 61,
      "Type": "ReceiptAdvice",
      "Timestamp": "2016-12-20T16:40:26.407+08:00",
      "LastChange": "2016-12-20T16:40:26.407+08:00",
      "State": "RECEIVED",
      "History": [],
      "HistoryAvailable": false,
      "UnifiedStateCausedByOtherParty": false,
      "Received": false,
      "AllowedActions": [],
      "Initiator": {
        "CompanyAccountId": "9b42f49e-028d-43cc-b6fa-6e24b2a43dc9",
        "CompanyAccountName": "중국어002公司",
        "UserId": "9f6a525d-0477-4036-9bc8-893cfebe726d",
        "UserName": "중국어002联系 002"
      },
      "PendingDocument": false,
      "Visible": false
    }
  ]
}
```

## 4: Get workflow result [TODO JD fill fullfill this] 
####  

## 5: Put some comments. 
####  

## 6: Approve or Reject a proforma
####  localhost:8888/tradeshift-backend/rest/external/documents/08000000-a87f-53da-95b7-476222200021?documentProfileId=tradeshift.status.1.0
```javascript
{
   "DocumentResponse":[
      {
         "Response":{
            "ReferenceID":{
               "value":"1"
            },
            "ResponseCode":{
               "value":"BusinessAccept"
            }
         },
         "DocumentReference":{
            "UUID":{
               "value":"4613cdde-ce51-58c2-a0eb-8558fdbdbb3c"
            },
            "ID":{
               "value":"000021"
            }
         }
      }
   ],
   "ID":{
      "value":"08000000-a87f-53da-95b7-476222200021"
   },
   "CustomizationID":{
      "value":"urn:tradeshift.com:ubl-2.0-customizations:2010-06"
   },
   "IssueDate":{
      "value":"2016-12-12"
   },
   "ProfileID":{
      "value":"urn:www.cenbii.eu:profile:bii04:ver1.0"
   },
   "SenderParty":{
      "Contact":{
         "Note":{
            "value":""
         }
      }
   },
   "ReceiverParty":{
      "Contact":{
         "Note":{
            "value":""
         }
      }
   },
   "DocumentType":"ApplicationResponseType"
}
```
