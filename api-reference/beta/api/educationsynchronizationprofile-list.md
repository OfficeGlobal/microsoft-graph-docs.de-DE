---
title: Liste educationSynchronizationProfiles
description: Abrufen der Auflistung der Schule Daten Synchronisierungsprofile in den Mandanten an.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1907b0ef08473a79d66e79fcb4751b281e9a18ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509553"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="55d0f-103">Liste educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="55d0f-103">List educationSynchronizationProfiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55d0f-104">Abrufen der Auflistung der Schule Daten [Profile Synchronization](../resources/educationsynchronizationprofile.md) in den Mandanten an.</span><span class="sxs-lookup"><span data-stu-id="55d0f-104">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="55d0f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="55d0f-105">Permissions</span></span>
<span data-ttu-id="55d0f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55d0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55d0f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="55d0f-108">Permission type</span></span> | <span data-ttu-id="55d0f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="55d0f-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="55d0f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="55d0f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55d0f-111">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55d0f-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="55d0f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="55d0f-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="55d0f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55d0f-113">Not supported.</span></span>|
|<span data-ttu-id="55d0f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="55d0f-114">Application</span></span>|<span data-ttu-id="55d0f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55d0f-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55d0f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55d0f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55d0f-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="55d0f-117">Optional query parameters</span></span>
<span data-ttu-id="55d0f-118">Diese Methode unterstützt die folgenden [Parameter für OData-Abfrage](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen: $filter, $orderby, $top, $skip und $count.</span><span class="sxs-lookup"><span data-stu-id="55d0f-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55d0f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55d0f-119">Request headers</span></span>
| <span data-ttu-id="55d0f-120">Name</span><span class="sxs-lookup"><span data-stu-id="55d0f-120">Name</span></span>       | <span data-ttu-id="55d0f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="55d0f-121">Type</span></span> | <span data-ttu-id="55d0f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55d0f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="55d0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55d0f-123">Authorization</span></span>  | <span data-ttu-id="55d0f-124">string</span><span class="sxs-lookup"><span data-stu-id="55d0f-124">string</span></span>  | <span data-ttu-id="55d0f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55d0f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55d0f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55d0f-127">Request body</span></span>
<span data-ttu-id="55d0f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="55d0f-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="55d0f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="55d0f-129">Response</span></span>
<span data-ttu-id="55d0f-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="55d0f-130">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55d0f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55d0f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55d0f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55d0f-132">Request</span></span>
<span data-ttu-id="55d0f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="55d0f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="55d0f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="55d0f-134">Response</span></span>
<span data-ttu-id="55d0f-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="55d0f-135">The following is an example of the response.</span></span> 

><span data-ttu-id="55d0f-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="55d0f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
