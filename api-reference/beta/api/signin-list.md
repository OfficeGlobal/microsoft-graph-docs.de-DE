---
title: Liste signIns
description: Ruft die Azure AD Benutzer Anmeldungen für Ihre Mandanten. In den Protokollen-Anmeldung sind derzeit interaktiv in Art sind (wobei ein Benutzername und Kennwort als Teil des Autorisierungstoken übergeben wird) und erfolgreicher federated Anmeldungen Anmeldevorgängen enthalten.  Die neuesten SignIns werden zuerst zurückgegeben.
localization_priority: Priority
ms.openlocfilehash: 8596bd168a3e10cbea9e15e2f61d6bd668fd27b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861789"
---
# <a name="list-signins"></a><span data-ttu-id="f7dd1-105">Liste signIns</span><span class="sxs-lookup"><span data-stu-id="f7dd1-105">List signIns</span></span>

<span data-ttu-id="f7dd1-106">Ruft die Azure AD Benutzer Anmeldungen für Ihre Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="f7dd1-107">In den Protokollen-Anmeldung sind derzeit interaktiv in Art sind (wobei ein Benutzername und Kennwort als Teil des Autorisierungstoken übergeben wird) und erfolgreicher federated Anmeldungen Anmeldevorgängen enthalten.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="f7dd1-108">Die neuesten SignIns werden zuerst zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="f7dd1-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7dd1-109">Permissions</span></span>
<span data-ttu-id="f7dd1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7dd1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7dd1-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7dd1-112">Permission type</span></span>      | <span data-ttu-id="f7dd1-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7dd1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7dd1-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7dd1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f7dd1-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7dd1-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="f7dd1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7dd1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7dd1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7dd1-117">Not supported</span></span>   |
|<span data-ttu-id="f7dd1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7dd1-118">Application</span></span> | <span data-ttu-id="f7dd1-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7dd1-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="f7dd1-120">Darüber hinaus müssen apps Azure AD [ordnungsgemäß registriert](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) sein.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="f7dd1-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7dd1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7dd1-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f7dd1-122">Optional query parameters</span></span>
<span data-ttu-id="f7dd1-123">Diese Methode unterstützt die folgende OData-Abfrageparameter zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="f7dd1-124">Überprüfen Sie die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) dafür, wie diese Parameter zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="f7dd1-125">Name</span><span class="sxs-lookup"><span data-stu-id="f7dd1-125">Name</span></span>     |<span data-ttu-id="f7dd1-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7dd1-126">Description</span></span>                            |<span data-ttu-id="f7dd1-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7dd1-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="f7dd1-128">$filter</span><span class="sxs-lookup"><span data-stu-id="f7dd1-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="f7dd1-129">Dient zum Filtern von Ergebnissen (Zeilen).</span><span class="sxs-lookup"><span data-stu-id="f7dd1-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="f7dd1-130">$top</span><span class="sxs-lookup"><span data-stu-id="f7dd1-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="f7dd1-131">Dient zum Festlegen der Seitengröße von Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="f7dd1-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f7dd1-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="f7dd1-133">Ruft ab, das die nächste Seite mit Ergebnissen aus Ergebnis, die festgelegt über mehrere Seiten erstrecken.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="f7dd1-134">Liste der Attribute von $filter Parameter unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="f7dd1-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="f7dd1-135">Name des Attributs</span><span class="sxs-lookup"><span data-stu-id="f7dd1-135">Attribute Name</span></span> |<span data-ttu-id="f7dd1-136">Unterstützte Operatoren</span><span class="sxs-lookup"><span data-stu-id="f7dd1-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="f7dd1-137">id</span><span class="sxs-lookup"><span data-stu-id="f7dd1-137">id</span></span>|<span data-ttu-id="f7dd1-138">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-138">eq</span></span>|
|<span data-ttu-id="f7dd1-139">userId</span><span class="sxs-lookup"><span data-stu-id="f7dd1-139">userId</span></span>|<span data-ttu-id="f7dd1-140">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-140">eq</span></span>|
|<span data-ttu-id="f7dd1-141">appId</span><span class="sxs-lookup"><span data-stu-id="f7dd1-141">appId</span></span>|<span data-ttu-id="f7dd1-142">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-142">eq</span></span>|
|<span data-ttu-id="f7dd1-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7dd1-143">createdDateTime</span></span>| <span data-ttu-id="f7dd1-144">EQ le ge</span><span class="sxs-lookup"><span data-stu-id="f7dd1-144">eq, le, ge</span></span>|
|<span data-ttu-id="f7dd1-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f7dd1-145">userDisplayName</span></span>| <span data-ttu-id="f7dd1-146">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-146">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f7dd1-147">userPrincipalName</span></span>| <span data-ttu-id="f7dd1-148">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-148">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f7dd1-149">appDisplayName</span></span>| <span data-ttu-id="f7dd1-150">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-150">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f7dd1-151">ipAddress</span></span>| <span data-ttu-id="f7dd1-152">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-152">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-153">/ Ortsname des Standorts</span><span class="sxs-lookup"><span data-stu-id="f7dd1-153">location/city</span></span>| <span data-ttu-id="f7dd1-154">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-154">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-155">Speicherort/Status</span><span class="sxs-lookup"><span data-stu-id="f7dd1-155">location/state</span></span>| <span data-ttu-id="f7dd1-156">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-156">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-157">Speicherort/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f7dd1-157">location/countryOrRegion</span></span>| <span data-ttu-id="f7dd1-158">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-158">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-159">Status/errorCode</span><span class="sxs-lookup"><span data-stu-id="f7dd1-159">status/errorCode</span></span>|<span data-ttu-id="f7dd1-160">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-160">eq</span></span>|
|<span data-ttu-id="f7dd1-161">InitiatedBy/Mitgliedsname</span><span class="sxs-lookup"><span data-stu-id="f7dd1-161">initiatedBy/user/id</span></span>|<span data-ttu-id="f7dd1-162">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-162">eq</span></span>|
|<span data-ttu-id="f7dd1-163">InitiatedBy/Benutzer/displayName</span><span class="sxs-lookup"><span data-stu-id="f7dd1-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="f7dd1-164">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-164">eq</span></span>|
|<span data-ttu-id="f7dd1-165">InitiatedBy/Benutzer/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f7dd1-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="f7dd1-166">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-166">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="f7dd1-167">clientAppUsed</span></span>| <span data-ttu-id="f7dd1-168">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-168">eq</span></span>|
|<span data-ttu-id="f7dd1-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="f7dd1-169">conditionalAccessStatus</span></span> | <span data-ttu-id="f7dd1-170">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-170">eq</span></span>|
|<span data-ttu-id="f7dd1-171">DeviceDetail-browser</span><span class="sxs-lookup"><span data-stu-id="f7dd1-171">deviceDetail/browser</span></span>| <span data-ttu-id="f7dd1-172">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-172">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-173">DeviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f7dd1-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="f7dd1-174">EQ startswith</span><span class="sxs-lookup"><span data-stu-id="f7dd1-174">eq, startswith</span></span>|
|<span data-ttu-id="f7dd1-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="f7dd1-175">correlationId</span></span>| <span data-ttu-id="f7dd1-176">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-176">eq</span></span>|
|<span data-ttu-id="f7dd1-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="f7dd1-177">riskDetail</span></span>| <span data-ttu-id="f7dd1-178">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-178">eq</span></span>|
|<span data-ttu-id="f7dd1-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="f7dd1-179">riskLevelAggregated</span></span>| <span data-ttu-id="f7dd1-180">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-180">eq</span></span>|
|<span data-ttu-id="f7dd1-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="f7dd1-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="f7dd1-182">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-182">eq</span></span>|
|<span data-ttu-id="f7dd1-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="f7dd1-183">riskEventTypes</span></span>| <span data-ttu-id="f7dd1-184">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-184">eq</span></span>|
|<span data-ttu-id="f7dd1-185">riskState</span><span class="sxs-lookup"><span data-stu-id="f7dd1-185">riskState</span></span>| <span data-ttu-id="f7dd1-186">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-186">eq</span></span>|
|<span data-ttu-id="f7dd1-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="f7dd1-187">originalRequestId</span></span>| <span data-ttu-id="f7dd1-188">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-188">eq</span></span>|
|<span data-ttu-id="f7dd1-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="f7dd1-189">tokenIssuerName</span></span>| <span data-ttu-id="f7dd1-190">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-190">eq</span></span>|
|<span data-ttu-id="f7dd1-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="f7dd1-191">tokenIssuerType</span></span>| <span data-ttu-id="f7dd1-192">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-192">eq</span></span>|
|<span data-ttu-id="f7dd1-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f7dd1-193">resourceDisplayName</span></span>| <span data-ttu-id="f7dd1-194">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-194">eq</span></span>|
|<span data-ttu-id="f7dd1-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="f7dd1-195">resourceId</span></span>| <span data-ttu-id="f7dd1-196">eq</span><span class="sxs-lookup"><span data-stu-id="f7dd1-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="f7dd1-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7dd1-197">Response</span></span>
<span data-ttu-id="f7dd1-198">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Anmelden](../resources/signin.md) .</span><span class="sxs-lookup"><span data-stu-id="f7dd1-198">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7dd1-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7dd1-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7dd1-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7dd1-200">Request</span></span>
<span data-ttu-id="f7dd1-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="f7dd1-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7dd1-202">Response</span></span>
<span data-ttu-id="f7dd1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7dd1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
