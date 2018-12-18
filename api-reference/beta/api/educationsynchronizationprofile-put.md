---
title: Aktualisieren einer educationSynchronizationProfile
description: Aktualisieren Sie die Eigenschaften für ein vorhandenes Schule Daten Synchronisierung Profil im Mandanten.
author: mmast-msft
ms.openlocfilehash: 17bf46eb4ebd6783f7bafba828ff1bcb7ad5ac48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361467"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="66550-103">Aktualisieren einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="66550-103">Update an educationSynchronizationProfile</span></span>

> <span data-ttu-id="66550-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66550-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66550-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66550-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66550-106">Aktualisieren Sie die Eigenschaften für ein vorhandenes Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="66550-106">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="66550-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="66550-107">Permissions</span></span>
<span data-ttu-id="66550-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66550-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66550-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66550-110">Permission type</span></span> | <span data-ttu-id="66550-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="66550-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="66550-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66550-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66550-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66550-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="66550-114">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="66550-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="66550-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66550-115">Not supported.</span></span>|
|<span data-ttu-id="66550-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66550-116">Application</span></span>|<span data-ttu-id="66550-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66550-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66550-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66550-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="66550-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66550-119">Request headers</span></span>
| <span data-ttu-id="66550-120">Name</span><span class="sxs-lookup"><span data-stu-id="66550-120">Name</span></span>       | <span data-ttu-id="66550-121">Typ</span><span class="sxs-lookup"><span data-stu-id="66550-121">Type</span></span> | <span data-ttu-id="66550-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66550-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66550-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="66550-123">Authorization</span></span>  | <span data-ttu-id="66550-124">string</span><span class="sxs-lookup"><span data-stu-id="66550-124">string</span></span>  | <span data-ttu-id="66550-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="66550-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="66550-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66550-127">Content-Type</span></span> | <span data-ttu-id="66550-128">string</span><span class="sxs-lookup"><span data-stu-id="66550-128">string</span></span> | <span data-ttu-id="66550-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="66550-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66550-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66550-131">Request body</span></span>
<span data-ttu-id="66550-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [SynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="66550-132">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66550-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="66550-133">Response</span></span>
<span data-ttu-id="66550-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `202, Accepted` Antwortcode und eines [SynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="66550-134">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66550-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66550-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66550-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66550-136">Request</span></span>
<span data-ttu-id="66550-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66550-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="66550-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="66550-138">Response</span></span>
<span data-ttu-id="66550-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="66550-139">Here is an example of the response.</span></span> 

><span data-ttu-id="66550-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="66550-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
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