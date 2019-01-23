---
title: Liste educationSynchronizationProfiles
description: Abrufen der Auflistung der Schule Daten Synchronisierungsprofile in den Mandanten an.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ed001a7c265f16057ea216d21f7a05f672df7065
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425071"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="dfdf4-103">Liste educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="dfdf4-103">List educationSynchronizationProfiles</span></span>

> <span data-ttu-id="dfdf4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfdf4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfdf4-106">Abrufen der Auflistung der Schule Daten [Profile Synchronization](../resources/educationsynchronizationprofile.md) in den Mandanten an.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-106">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfdf4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dfdf4-107">Permissions</span></span>
<span data-ttu-id="dfdf4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfdf4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfdf4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dfdf4-110">Permission type</span></span> | <span data-ttu-id="dfdf4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dfdf4-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="dfdf4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dfdf4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dfdf4-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfdf4-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="dfdf4-114">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="dfdf4-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="dfdf4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dfdf4-115">Not supported.</span></span>|
|<span data-ttu-id="dfdf4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dfdf4-116">Application</span></span>|<span data-ttu-id="dfdf4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dfdf4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfdf4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dfdf4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfdf4-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dfdf4-119">Optional query parameters</span></span>
<span data-ttu-id="dfdf4-120">Diese Methode unterstützt die folgenden [Parameter für OData-Abfrage](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen: $filter, $orderby, $top, $skip und $count.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-120">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfdf4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dfdf4-121">Request headers</span></span>
| <span data-ttu-id="dfdf4-122">Name</span><span class="sxs-lookup"><span data-stu-id="dfdf4-122">Name</span></span>       | <span data-ttu-id="dfdf4-123">Typ</span><span class="sxs-lookup"><span data-stu-id="dfdf4-123">Type</span></span> | <span data-ttu-id="dfdf4-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfdf4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dfdf4-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="dfdf4-125">Authorization</span></span>  | <span data-ttu-id="dfdf4-126">string</span><span class="sxs-lookup"><span data-stu-id="dfdf4-126">string</span></span>  | <span data-ttu-id="dfdf4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfdf4-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dfdf4-129">Request body</span></span>
<span data-ttu-id="dfdf4-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dfdf4-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="dfdf4-131">Response</span></span>
<span data-ttu-id="dfdf4-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="dfdf4-132">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfdf4-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dfdf4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfdf4-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dfdf4-134">Request</span></span>
<span data-ttu-id="dfdf4-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="dfdf4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="dfdf4-136">Response</span></span>
<span data-ttu-id="dfdf4-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-137">The following is an example of the response.</span></span> 

><span data-ttu-id="dfdf4-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="dfdf4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3296

{
    "value": [
    {
        "displayName": "Test Profile",
        "state": "provisioned",
        "id": "15e9b9fa-de85-492e-aa44-550c40de626e",
        "dataProvider": {
            "@odata.type": "microsoft.graph.educationCsvDataProvider",
            "customizations": {
                "school": {
                    "optionalPropertiesToSync": [
                        "School NCES_ID",
                        "State ID",
                        "GradeLow",
                        "GradeHigh",
                        "Principal Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "section": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "student": {
                    "optionalPropertiesToSync": [
                        "State ID",
                        "Email",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacher": {
                    "optionalPropertiesToSync": [
                        "Teacher Number",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "studentEnrollment": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacherRoster": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                }
            }
        },
        "identitySynchronizationConfiguration": {
            "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
            "userDomains": [
                {
                    "appliesTo": "student",
                    "name": "testschool.edu"
                },
                {
                    "appliesTo": "teacher",
                    "name": "testschool.edu"
                }
            ]
        },
        "licensesToAssign": [
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",                
                "appliesTo": "teacher",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            },
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
                "appliesTo": "student",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            }
        ]
    }
  ]
}
```
