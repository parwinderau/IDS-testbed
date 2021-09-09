# Test Cases 
**ids3c-co:TCS_AUD_01_AccessControlLogging**
    a                       ids3cm:ComponentTestCaseSpecification ;
    rdfs:label              "TODO : rdfs:label"@en ;
    dct:description         """TODO : description : TCS_AUD_01_AccessControlLogging"""@en ;
    
    
**TODO 	ids3cm:testDesignSpecificStrategyType	ids3c-co:TDS_AUD_01_AccessControlLogging_BaseSecurityProfile_ChecklistApproach ;**

**TODO 	ids3cm:testDesignSpecificStrategyType	ids3c-co:TDS_AUD_01_AccessControlLogging_BaseSecurityProfile_ConceptReview ;**

**TODO 	ids3cm:testDesignSpecificStrategyType	ids3c-co:TDS_AUD_01_AccessControlLogging_TrustSecurityProfile_ConceptReview ;**

**TODO 	ids3cm:testDesignSpecificStrategyType	ids3c-co:TDS_AUD_01_AccessControlLogging_TrustSecurityProfile_HighAssuranceEvaluation ;**

**TODO 	ids3cm:testDesignSpecificStrategyType	ids3c-co:TDS_AUD_01_AccessControlLogging_TrustPlusSecurityProfile_ConceptReview ;**

**TODO 	ids3cm:testDesignSpecificStrategyType	ids3c-co:TDS_AUD_01_AccessControlLogging_TrustPlusSecurityProfile_HighAssuranceEvaluation ;**

TODO: set <ids3cm:UNSPECIFIED> to <ids3cm:CONSUMER> OR <ids3cm:PROVIDER>

    ids3cm:testRole         ids3cm:UNSPECIFIED ;
    ids3cm:initialCondition [ a               ids3cm:InitialCondition ;
                              ## TODO rdfs:label	"TODO:" ;
                              dct:description """TODO:"""@en ;
                            ## TODO ids3cm:testCaseSpecification	ids3cm:XYZ_ABC_Schokolade ;
                            ] ;
TODO 	ids3cm:testConfig	[ a ids3cm:TestConfig ; ] ;

    ids3cm:trigger          """TODO : trigger"""@en ;
    ids3cm:expectedBehavior """TODO : a expected behavior"""@en ;
    ids3cm:finalCondition   [ a               ids3cm:FinalCondition ;
                              ## TODO rdfs:label	"TODO:" ;
                              dct:description """TODO:"""@en ;
                            ## TODO ids3cm:testCaseSpecification	ids3cm:ABC_XYZ_Marzipan ;
                            ] ;
                            
TODO 	rdfs:comment	"""TODO : rdfs:comment"""@en ;

## TO FILL
* testRole
* initialCondition
* testConfig
* trigger
* expectedBehavior
* finalCondition
* comment
## Possible Scenarios
1. TEST_DEPLOYMENT
2. PRODUCTIVE_DEPLOYMENT
---
1. LOCALHOST CERT
2. EXPIRED CERT
3. VALID CERT
4. UNRECOGNIZED CERT by DAPS
---
1. VALID DAPS ENDPOINT
2. INVALID DAPS ENDPOINT
---
1. VALID BROKER ENDPOINT
1. INVALID BROKER ENDPOINT
### Scenarios
* 1111 TEST_DEPLOYMENT + LOCALHOST CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT   
* 1112 TEST_DEPLOYMENT + LOCALHOST CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                  
* 1121 TEST_DEPLOYMENT + LOCALHOST CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT  
* 1122 TEST_DEPLOYMENT + LOCALHOST CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                       
* 1211 TEST_DEPLOYMENT + EXPIRED CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
* 1212 TEST_DEPLOYMENT + EXPIRED CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                             
* 1221 TEST_DEPLOYMENT + EXPIRED CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT 
* 1222 TEST_DEPLOYMENT + EXPIRED CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                        
* 1311 TEST_DEPLOYMENT + VALID CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT   
* 1312 TEST_DEPLOYMENT + VALID CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                           
* 1321 TEST_DEPLOYMENT + VALID CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT    
* 1322 TEST_DEPLOYMENT + VALID CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                       
* 1411 TEST_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
* 1412 TEST_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT             
* 1421 TEST_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT  
* 1422 TEST_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                 
* 2111 PRODUCTIVE_DEPLOYMENT + LOCALHOST CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT 
* 2112 PRODUCTIVE_DEPLOYMENT + LOCALHOST CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                             
* 2121 PRODUCTIVE_DEPLOYMENT + LOCALHOST CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT   
* 2122 PRODUCTIVE_DEPLOYMENT + LOCALHOST CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT               
* 2211 PRODUCTIVE_DEPLOYMENT + EXPIRED CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT     
* 2212 PRODUCTIVE_DEPLOYMENT + EXPIRED CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                       
* 2221 PRODUCTIVE_DEPLOYMENT + EXPIRED CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT     
* 2222 PRODUCTIVE_DEPLOYMENT + EXPIRED CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT               
* 2311 PRODUCTIVE_DEPLOYMENT + VALID CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT  
* 2312 PRODUCTIVE_DEPLOYMENT + VALID CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                       
* 2321 PRODUCTIVE_DEPLOYMENT + VALID CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT       
* 2322 PRODUCTIVE_DEPLOYMENT + VALID CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT                         
* 2411 PRODUCTIVE_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT   
* 2412 PRODUCTIVE_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT        
* 2421 PRODUCTIVE_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
* 2422 PRODUCTIVE_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT   

## Content
#### testRole
#### initialCondition
#### testConfig
#### trigger
#### expected Behavior
#### finalCondition
#### comment

## Test Case(s)
### TS 000 (TODO)
Lanzar el dsc

### TS 1111 TEST_DEPLOYMENT + LOCALHOST CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000 
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behaviorhttps://broker.ids.isst.fraunhofer.de/infrastructure
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 1112 TEST_DEPLOYMENT + LOCALHOST CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000 
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 

daps.token.url=https://daps.aisec.fraunhofer.de

daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 1121 TEST_DEPLOYMENT + LOCALHOST CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 

ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.badenpoint/test
daps.key.url=https://daps.badenpoint/test/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 1122 TEST_DEPLOYMENT + LOCALHOST CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.badenpoint/test
daps.key.url=https://daps.badenpoint/test/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 1211 TEST_DEPLOYMENT + EXPIRED CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : testidsa9.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
Code 200 with message type > @type : "ids:MessageProcessedNotificationMessage"
#### finalCondition
#### comment

### TS 1212 TEST_DEPLOYMENT + EXPIRED CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : testidsa9.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
Code 500 with Response Body : Ids message handling failed. {broker url}: Name or service unknown
#### finalCondition
#### comment

### TS 1221 TEST_DEPLOYMENT + EXPIRED CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : testidsa9.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
#### finalCondition
#### comment

### TS 1222 TEST_DEPLOYMENT + EXPIRED CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : testidsa9.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
#### finalCondition
#### comment

### TS 1311 TEST_DEPLOYMENT + VALID CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 1312 TEST_DEPLOYMENT + VALID CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 1321 TEST_DEPLOYMENT + VALID CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
A rejection message regarding the validity of the certificate
#### finalCondition
#### comment

### TS 1322 TEST_DEPLOYMENT + VALID CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
Error retrieving token: {DAPS_URL}
#### finalCondition
#### comment

### TS 1411 TEST_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
Response body of token request: {"access_token":"..."}
#### finalCondition
#### comment

### TS 1412 TEST_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
Error retrieving token : {DAPS_URL}
#### finalCondition
#### comment

### TS 1421 TEST_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
#### finalCondition
#### comment

### TS 1422 TEST_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
#### finalCondition
#### comment

### TS 2111 PRODUCTIVE_DEPLOYMENT + LOCALHOST CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000 
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 2112 PRODUCTIVE_DEPLOYMENT + LOCALHOST CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000 
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 2121 PRODUCTIVE_DEPLOYMENT + LOCALHOST CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
A rejection message regarding the validity of the certificate
#### finalCondition
#### comment

### TS 2122 PRODUCTIVE_DEPLOYMENT + LOCALHOST CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
A rejection message of type "NOT_AUTHENTICATED"
Error retrieving token: {DAPS_URL}
#### finalCondition
#### comment

### TS 2211 TEST_DEPLOYMENT + EXPIRED CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
Response body of token request: {"access_token":"..."}
#### finalCondition
#### comment

### TS 2212 PRODUCTIVE_DEPLOYMENT + EXPIRED CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
Error retrieving token : {DAPS_URL}
#### finalCondition
#### comment

### TS 2221 PRODUCTIVE_DEPLOYMENT + EXPIRED CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
#### finalCondition
#### comment

### TS 2222 PRODUCTIVE_DEPLOYMENT + EXPIRED CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
#### finalCondition
#### comment

### TS 2311 PRODUCTIVE_DEPLOYMENT + VALID CERT + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 2312 PRODUCTIVE_DEPLOYMENT + VALID CERT + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
ERROR - Certificate of the Connector is missing aki/ski extensions!
#### finalCondition
#### comment

### TS 2321 PRODUCTIVE_DEPLOYMENT + VALID CERT + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
A rejection message regarding the validity of the certificate
#### finalCondition
#### comment

### TS 2322 PRODUCTIVE_DEPLOYMENT + VALID CERT + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
Error retrieving token: {DAPS_URL}
#### finalCondition
#### comment

### TS 2411 PRODUCTIVE_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + VALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
Response body of token request: {"access_token":"..."}
#### finalCondition
#### comment

### TS 2412 PRODUCTIVE_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + VALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
Error retrieving token : {DAPS_URL}
#### finalCondition
#### comment

### TS 2421 PRODUCTIVE_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + INVALID DAPS ENDPOINT + VALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json

#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.ids.isst.fraunhofer.de/infrastructure
#### expected Behavior
#### finalCondition
#### comment

### TS 2422 PRODUCTIVE_DEPLOYMENT + UNRECOGNIZED CERT by DAPS + INVALID DAPS ENDPOINT + INVALID BROKER ENDPOINT
#### testRole
#### initial Condition
Referencia TS 000
#### testConfig
/src/main/resources/conf/config.json > 
ids:connectorDeployMode : TEST_DEPLOYMENT
ids:keyStore : keystore-localhost.p12

/src/main/resources/application.properties > 
daps.token.url=https://daps.aisec.fraunhofer.de
daps.key.url=https://daps.aisec.fraunhofer.de/v2/.well-known/jwks.json
#### trigger
Execute the "POST /api/ids/connector/update" call in the Dataspace Connector API with url: https://broker.badenpoint/test
#### expected Behavior
#### finalCondition
#### comment