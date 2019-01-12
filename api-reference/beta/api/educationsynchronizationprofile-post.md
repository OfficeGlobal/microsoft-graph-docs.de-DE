---
title: Erstellen einer educationSynchronizationProfile
description: 'Erstellen Sie eine Anforderung für ein neues Schule Daten Synchronisierung Profil im Mandanten. Abfragen des Status, um den Status des Profils abzurufen. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9d471766a8492e03809d05d6d0366c8e44d59015
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915760"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="632ed-104">Erstellen einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="632ed-104">Create an educationSynchronizationProfile</span></span>

> <span data-ttu-id="632ed-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="632ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="632ed-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="632ed-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="632ed-107">Erstellen Sie eine Anforderung für ein neues Schule Daten [Profile Synchronization](../resources/educationsynchronizationprofile.md) in den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="632ed-107">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="632ed-108">[Abfrage der Status](educationsynchronizationprofilestatus-get.md) den Status des Profils abgerufen.</span><span class="sxs-lookup"><span data-stu-id="632ed-108">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="632ed-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="632ed-109">Permissions</span></span>
<span data-ttu-id="632ed-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="632ed-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="632ed-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="632ed-112">Permission type</span></span> | <span data-ttu-id="632ed-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="632ed-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="632ed-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="632ed-114">Delegated (work or school account)</span></span> | <span data-ttu-id="632ed-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="632ed-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="632ed-116">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="632ed-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="632ed-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="632ed-117">Not supported.</span></span>|
|<span data-ttu-id="632ed-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="632ed-118">Application</span></span>|<span data-ttu-id="632ed-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="632ed-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="632ed-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="632ed-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="632ed-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="632ed-121">Request headers</span></span>
| <span data-ttu-id="632ed-122">Name</span><span class="sxs-lookup"><span data-stu-id="632ed-122">Name</span></span>       | <span data-ttu-id="632ed-123">Typ</span><span class="sxs-lookup"><span data-stu-id="632ed-123">Type</span></span> | <span data-ttu-id="632ed-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="632ed-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="632ed-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="632ed-125">Authorization</span></span>  | <span data-ttu-id="632ed-126">string</span><span class="sxs-lookup"><span data-stu-id="632ed-126">string</span></span>  | <span data-ttu-id="632ed-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="632ed-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="632ed-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="632ed-129">Content-Type</span></span> | <span data-ttu-id="632ed-130">string</span><span class="sxs-lookup"><span data-stu-id="632ed-130">string</span></span> | <span data-ttu-id="632ed-131">Application/Json.</span><span class="sxs-lookup"><span data-stu-id="632ed-131">Application/json.</span></span> <span data-ttu-id="632ed-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="632ed-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="632ed-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="632ed-133">Request body</span></span>
<span data-ttu-id="632ed-134">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="632ed-134">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="632ed-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="632ed-135">Response</span></span>
<span data-ttu-id="632ed-136">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `202, Accepted` Antwortcode und eines [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="632ed-136">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="632ed-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="632ed-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="632ed-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="632ed-138">Request</span></span>
<span data-ttu-id="632ed-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="632ed-139">The following is an example of the request.</span></span>
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
        "@odata.type": "#microsoft.graph.educationcsvdataprovider",
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
        "@odata.type": "#microsoft.graph.educationidentitycreationconfiguration",
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

##### <a name="response"></a><span data-ttu-id="632ed-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="632ed-140">Response</span></span>
<span data-ttu-id="632ed-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="632ed-141">The following is an example of the response.</span></span> 

><span data-ttu-id="632ed-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="632ed-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "#microsoft.graph.educationCsvDataProvider",
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
        "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
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
            "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```
