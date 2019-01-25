---
title: Erstellen einer educationSynchronizationProfile
description: 'Erstellen Sie eine Anforderung für ein neues Schule Daten Synchronisierung Profil im Mandanten. Abfragen des Status, um den Status des Profils abzurufen. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: efc9b76405b57d0e47d645d0e7b00dc9425ba71b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520816"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="4e273-104">Erstellen einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="4e273-104">Create an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e273-105">Erstellen Sie eine Anforderung für ein neues Schule Daten [Profile Synchronization](../resources/educationsynchronizationprofile.md) in den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4e273-105">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="4e273-106">[Abfrage der Status](educationsynchronizationprofilestatus-get.md) den Status des Profils abgerufen.</span><span class="sxs-lookup"><span data-stu-id="4e273-106">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4e273-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4e273-107">Permissions</span></span>
<span data-ttu-id="4e273-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e273-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e273-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e273-110">Permission type</span></span> | <span data-ttu-id="4e273-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4e273-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4e273-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e273-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e273-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e273-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="4e273-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e273-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4e273-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e273-115">Not supported.</span></span>|
|<span data-ttu-id="4e273-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e273-116">Application</span></span>|<span data-ttu-id="4e273-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e273-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e273-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e273-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="4e273-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e273-119">Request headers</span></span>
| <span data-ttu-id="4e273-120">Name</span><span class="sxs-lookup"><span data-stu-id="4e273-120">Name</span></span>       | <span data-ttu-id="4e273-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4e273-121">Type</span></span> | <span data-ttu-id="4e273-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e273-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4e273-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e273-123">Authorization</span></span>  | <span data-ttu-id="4e273-124">string</span><span class="sxs-lookup"><span data-stu-id="4e273-124">string</span></span>  | <span data-ttu-id="4e273-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4e273-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4e273-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e273-127">Content-Type</span></span> | <span data-ttu-id="4e273-128">string</span><span class="sxs-lookup"><span data-stu-id="4e273-128">string</span></span> | <span data-ttu-id="4e273-129">application/json</span><span class="sxs-lookup"><span data-stu-id="4e273-129">Application/json.</span></span> <span data-ttu-id="4e273-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4e273-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e273-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e273-131">Request body</span></span>
<span data-ttu-id="4e273-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e273-132">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4e273-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e273-133">Response</span></span>
<span data-ttu-id="4e273-134">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `202, Accepted` Antwortcode und eines [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4e273-134">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e273-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e273-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e273-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e273-136">Request</span></span>
<span data-ttu-id="4e273-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e273-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationSynchronizationProfile"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
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
        "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration",
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

##### <a name="response"></a><span data-ttu-id="4e273-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e273-138">Response</span></span>
<span data-ttu-id="4e273-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4e273-139">The following is an example of the response.</span></span> 

><span data-ttu-id="4e273-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4e273-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 201 Created
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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
