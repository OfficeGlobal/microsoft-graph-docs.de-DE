---
title: Erstellen einer educationSynchronizationProfile
description: 'Erstellen Sie eine Anforderung für ein neues Schule Daten Synchronisierung Profil im Mandanten. Abfragen des Status, um den Status des Profils abzurufen. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c5ce12f43af4e32691c34038a9a0c0527d314c06
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853851"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="d748a-104">Erstellen einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="d748a-104">Create an educationSynchronizationProfile</span></span>

> <span data-ttu-id="d748a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d748a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d748a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d748a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d748a-107">Erstellen Sie eine Anforderung für ein neues Schule Daten [Profile Synchronization](../resources/educationsynchronizationprofile.md) in den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d748a-107">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="d748a-108">[Abfrage der Status](educationsynchronizationprofilestatus-get.md) den Status des Profils abgerufen.</span><span class="sxs-lookup"><span data-stu-id="d748a-108">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d748a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d748a-109">Permissions</span></span>
<span data-ttu-id="d748a-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d748a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d748a-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d748a-112">Permission type</span></span> | <span data-ttu-id="d748a-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d748a-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="d748a-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d748a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d748a-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d748a-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="d748a-116">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="d748a-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d748a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d748a-117">Not supported.</span></span>|
|<span data-ttu-id="d748a-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d748a-118">Application</span></span>|<span data-ttu-id="d748a-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d748a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d748a-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d748a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d748a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d748a-121">Request headers</span></span>
| <span data-ttu-id="d748a-122">Name</span><span class="sxs-lookup"><span data-stu-id="d748a-122">Name</span></span>       | <span data-ttu-id="d748a-123">Typ</span><span class="sxs-lookup"><span data-stu-id="d748a-123">Type</span></span> | <span data-ttu-id="d748a-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d748a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d748a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d748a-125">Authorization</span></span>  | <span data-ttu-id="d748a-126">string</span><span class="sxs-lookup"><span data-stu-id="d748a-126">string</span></span>  | <span data-ttu-id="d748a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d748a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d748a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d748a-129">Content-Type</span></span> | <span data-ttu-id="d748a-130">string</span><span class="sxs-lookup"><span data-stu-id="d748a-130">string</span></span> | <span data-ttu-id="d748a-131">Application/Json.</span><span class="sxs-lookup"><span data-stu-id="d748a-131">Application/json.</span></span> <span data-ttu-id="d748a-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d748a-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d748a-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d748a-133">Request body</span></span>
<span data-ttu-id="d748a-134">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d748a-134">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d748a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d748a-135">Response</span></span>
<span data-ttu-id="d748a-136">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `202, Accepted` Antwortcode und eines [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d748a-136">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d748a-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d748a-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d748a-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d748a-138">Request</span></span>
<span data-ttu-id="d748a-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d748a-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d748a-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="d748a-140">Response</span></span>
<span data-ttu-id="d748a-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d748a-141">The following is an example of the response.</span></span> 

><span data-ttu-id="d748a-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d748a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
