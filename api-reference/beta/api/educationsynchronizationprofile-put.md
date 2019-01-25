---
title: Aktualisieren einer educationSynchronizationProfile
description: Aktualisieren Sie die Eigenschaften für ein vorhandenes Schule Daten Synchronisierung Profil im Mandanten.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 668aad65abe2c9b3d4609400118f9341748210f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510575"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="67001-103">Aktualisieren einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="67001-103">Update an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67001-104">Aktualisieren Sie die Eigenschaften für ein vorhandenes Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="67001-104">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="67001-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67001-105">Permissions</span></span>
<span data-ttu-id="67001-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67001-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67001-108">Permission type</span></span> | <span data-ttu-id="67001-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67001-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="67001-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67001-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67001-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67001-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="67001-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67001-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="67001-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67001-113">Not supported.</span></span>|
|<span data-ttu-id="67001-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67001-114">Application</span></span>|<span data-ttu-id="67001-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67001-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67001-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67001-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="67001-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67001-117">Request headers</span></span>
| <span data-ttu-id="67001-118">Name</span><span class="sxs-lookup"><span data-stu-id="67001-118">Name</span></span>       | <span data-ttu-id="67001-119">Typ</span><span class="sxs-lookup"><span data-stu-id="67001-119">Type</span></span> | <span data-ttu-id="67001-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67001-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="67001-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67001-121">Authorization</span></span>  | <span data-ttu-id="67001-122">string</span><span class="sxs-lookup"><span data-stu-id="67001-122">string</span></span>  | <span data-ttu-id="67001-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67001-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="67001-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67001-125">Content-Type</span></span> | <span data-ttu-id="67001-126">string</span><span class="sxs-lookup"><span data-stu-id="67001-126">string</span></span> | <span data-ttu-id="67001-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="67001-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67001-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67001-129">Request body</span></span>
<span data-ttu-id="67001-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [SynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="67001-130">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="67001-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="67001-131">Response</span></span>
<span data-ttu-id="67001-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `202, Accepted` Antwortcode und eines [SynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="67001-132">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67001-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67001-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67001-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67001-134">Request</span></span>
<span data-ttu-id="67001-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67001-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_synchronizationProfile"
}-->
```http
PUT https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationcsvdataprovider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ]
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationidentitycreationconfiguration",
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
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="67001-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="67001-136">Response</span></span>
<span data-ttu-id="67001-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="67001-137">Here is an example of the response.</span></span> 

><span data-ttu-id="67001-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="67001-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacher": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Teacher Number",
                    "Status",
                    "Middle Name",
                    "Secondary Email",
                    "Title",
                    "Qualification"
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
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
