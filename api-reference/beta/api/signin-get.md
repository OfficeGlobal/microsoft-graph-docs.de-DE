---
title: Erste Anmeldung
description: Ruft die Azure AD Benutzer Anmeldungen für Ihre Mandanten. In den Protokollen-Anmeldung sind derzeit interaktiv in Art sind (wobei ein Benutzername und Kennwort als Teil des Autorisierungstoken übergeben wird) und erfolgreicher federated Anmeldungen Anmeldevorgängen enthalten.
ms.openlocfilehash: 1934af9b918dc976ef7f3fc6cdd21c04f6fcc705
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064380"
---
# <a name="get-signin"></a><span data-ttu-id="bfe44-104">Erste Anmeldung</span><span class="sxs-lookup"><span data-stu-id="bfe44-104">Get signIn</span></span>
<span data-ttu-id="bfe44-105">Ruft die Azure AD Benutzer Anmeldungen für Ihre Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bfe44-105">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="bfe44-106">In den Protokollen-Anmeldung sind derzeit interaktiv in Art sind (wobei ein Benutzername und Kennwort als Teil des Autorisierungstoken übergeben wird) und erfolgreicher federated Anmeldungen Anmeldevorgängen enthalten.</span><span class="sxs-lookup"><span data-stu-id="bfe44-106">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="bfe44-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bfe44-107">Permissions</span></span>
<span data-ttu-id="bfe44-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfe44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfe44-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfe44-110">Permission type</span></span>      | <span data-ttu-id="bfe44-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfe44-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfe44-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfe44-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bfe44-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfe44-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="bfe44-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfe44-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfe44-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfe44-115">Not supported</span></span>   |
|<span data-ttu-id="bfe44-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfe44-116">Application</span></span> | <span data-ttu-id="bfe44-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfe44-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="bfe44-118">Darüber hinaus müssen apps Azure AD [ordnungsgemäß registriert](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) sein.</span><span class="sxs-lookup"><span data-stu-id="bfe44-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="bfe44-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfe44-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfe44-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bfe44-120">Optional query parameters</span></span>
<span data-ttu-id="bfe44-121">Diese Methode unterstützt die folgende OData-Abfrageparameter zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bfe44-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="bfe44-122">Überprüfen Sie die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) dafür, wie diese Parameter zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="bfe44-122">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfe44-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfe44-123">Request headers</span></span>
| <span data-ttu-id="bfe44-124">Name</span><span class="sxs-lookup"><span data-stu-id="bfe44-124">Name</span></span>      |<span data-ttu-id="bfe44-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfe44-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfe44-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfe44-126">Authorization</span></span>  | <span data-ttu-id="bfe44-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bfe44-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfe44-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfe44-128">Request body</span></span>
<span data-ttu-id="bfe44-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bfe44-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bfe44-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfe44-130">Response</span></span>
<span data-ttu-id="bfe44-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [Anmeldung](../resources/signin.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bfe44-131">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfe44-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfe44-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfe44-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfe44-133">Request</span></span>
<span data-ttu-id="bfe44-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bfe44-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "reque|location/city| eq, startswith|
st",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
##### <a name="response"></a><span data-ttu-id="bfe44-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfe44-135">Response</span></span>
<span data-ttu-id="bfe44-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bfe44-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211
```
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id": "id",
        "createdDateTime": "2018-01-09T21:17:21.5077253Z",
        "userDisplayName": "Jamie Doe",
        "userPrincipalName": "jdoe@contoso.com",
        "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302",
        "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
        "appDisplayName": "Azure",
        "ipAddress": "127.0.0.1",
        "status": {
            "errorCode": 0,
            "failureReason": null,
            "additionalDetails": "SignIn Success & CA Sucess"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v1.0.2016.0",
            "isCompliant": true,
            "isManaged": true,
            "trustType": ""
        },
        "location": {
            "city": "Redmond",
            "state": "WA",
            "countryOrRegion": "USA",
            "geoCoordinates": {
                "altitude": 41.589,
                "latitude": 41.589,
                "longitude": -93.6151
            }
        },
        "mfaDetail": {
            "mfaAuthMethod": "Phone Auth",
            "mfaAuthDetail": null
        },
        "correlationId": "17c47d3c-593d-4d08-ac20-813892b87e42",
        "conditionalAccessApplied": true,
        "conditionalAccessPolicies": [{
            "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
            "displayName": "capPolicy",
            "enforcedAccessControls": ["MFA", "TOU"],
            "enforcedSessionControls": ["CloudAppSecurity"],
            "result": "success"
        }],
        "isRisky": false,
        "riskLevel": "low"
    }]
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->