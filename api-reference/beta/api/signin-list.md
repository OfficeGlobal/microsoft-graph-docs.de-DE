---
title: Liste signIns
description: Ruft die Azure AD Benutzer Anmeldungen für Ihre Mandanten. In den Protokollen-Anmeldung sind derzeit interaktiv in Art sind (wobei ein Benutzername und Kennwort als Teil des Autorisierungstoken übergeben wird) und erfolgreicher federated Anmeldungen Anmeldevorgängen enthalten.  Die neuesten SignIns werden zuerst zurückgegeben.
ms.openlocfilehash: 3abca59187dcc9667789e33bcefc1bcc51d5ab10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059756"
---
# <a name="list-signins"></a>Liste signIns

Ruft die Azure AD Benutzer Anmeldungen für Ihre Mandanten. In den Protokollen-Anmeldung sind derzeit interaktiv in Art sind (wobei ein Benutzername und Kennwort als Teil des Autorisierungstoken übergeben wird) und erfolgreicher federated Anmeldungen Anmeldevorgängen enthalten.  Die neuesten SignIns werden zuerst zurückgegeben.


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | AuditLog.Read.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt   |
|Anwendung | AuditLog.Read.All | 

Darüber hinaus müssen apps Azure AD [ordnungsgemäß registriert](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) sein.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die folgende OData-Abfrageparameter zur Anpassung der Antwort. Überprüfen Sie die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) dafür, wie diese Parameter zu verwenden.

|Name     |Beschreibung                            |Beispiel|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|Dient zum Filtern von Ergebnissen (Zeilen). |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|Dient zum Festlegen der Seitengröße von Ergebnissen.|`/auditLogs/signIns?$top=1`|
|[$skiptoken](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|Ruft ab, das die nächste Seite mit Ergebnissen aus Ergebnis, die festgelegt über mehrere Seiten erstrecken.|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>Liste der Attribute von $filter Parameter unterstützt werden
|Name des Attributs |Unterstützte Operatoren|
|:----------------|:------|
|id|eq|
|userId|eq|
|appId|eq|
|createdDateTime| EQ le ge|
|userDisplayName| EQ startswith|
|userPrincipalName| EQ startswith|
|appDisplayName| EQ startswith|
|ipAddress| EQ startswith|
|/ Ortsname des Standorts| EQ startswith|
|Speicherort/Status| EQ startswith|
|Speicherort/countryOrRegion| EQ startswith|
|Status/errorCode|eq|
|InitiatedBy/Mitgliedsname|eq|
|InitiatedBy/Benutzer/displayName| eq|
|InitiatedBy/Benutzer/userPrincipalName| EQ startswith|
|clientAppUsed| eq|
|conditionalAccessStatus | eq|
|DeviceDetail-browser| EQ startswith|
|DeviceDetail/operatingSystem| EQ startswith|
|correlationId| eq|
|riskDetail| eq|
|riskLevelAggregated| eq|
|riskLevelDuringSignIn| eq|
|riskEventTypes| eq|
|riskState| eq|
|originalRequestId| eq|
|tokenIssuerName| eq|
|tokenIssuerType| eq|
|resourceDisplayName| eq|
|resourceId| eq|


## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Anmelden](../resources/signin.md) .
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id":"b01b1726-0147-425e-a7f7-21f252050400",
        "createdDateTime":"2018-11-06T18:48:33.8527147Z",
        "userDisplayName":"Jon Doe",
         "userPrincipalName":"admin@aad171.ccsctp.net",
         "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
        "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
         "appDisplayName":"Azure Portal",
         "ipAddress":"207.254.19.10",
         "clientAppUsed":"Browser",
        "mfaDetail":null,
         "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
         "conditionalAccessStatus":"notApplied",
        "originalRequestId":null,
        "isInteractive":true,
        "tokenIssuerName":null,
        "tokenIssuerType":"AzureAD",
        "processingTimeInMilliseconds":0,
        "riskDetail":"none",
        "riskLevelAggregated":"none",
        "riskLevelDuringSignIn":"none",
        "riskState":"none",
        "riskEventTypes":[

        ],
        "resourceDisplayName":"windows azure service management api",
        "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
        "authenticationMethodsUsed":[

        ],
        "status":{
            "errorCode":50140,
            "failureReason":"This error occurred due to 'Keep me signed in' interrupt when the user was signing-in.",
            "additionalDetails":null
        },
        "deviceDetail":{
            "deviceId":null,
            "displayName":null,
            "operatingSystem":"Windows 7",
            "browser":"Chrome 63.0.3239",
            "isCompliant":null,
            "isManaged":null,
            "trustType":null
        },
        "location":{
            "city":"Lithia Springs",
            "state":"Georgia",
            "countryOrRegion":"US",
            "geoCoordinates":{
                "altitude":null,
                "latitude":33.7930908203125,
                "longitude":-84.445358276367188
            }
        },
        "appliedConditionalAccessPolicies":[
            {
            "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
            "displayName":"New Name here4",
            "enforcedGrantControls":[
                "Mfa",
                "RequireCompliantDevice"
            ],
            "enforcedSessionControls":[

            ],
            "result":"notApplied"
            },
            {
            "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
            "displayName":"PipelineTest4",
            "enforcedGrantControls":[

            ],
            "enforcedSessionControls":[

            ],
            "result":"notEnabled"
            }
        ],
        "authenticationProcessingDetails":[

        ],
        "networkLocationDetails":[

        ]
        }
    
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
