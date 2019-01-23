---
title: Abrufen eines educationSynchronizationProfile
description: Rufen Sie ein Schule Synchronisierung Datenprofil im Mandanten auf Grundlage des Bezeichners ab.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0c4d06583b7ba892cf2ae4bddd8de16cd8612082
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406332"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="9a2fe-103">Abrufen eines educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="9a2fe-103">Get an educationSynchronizationProfile</span></span>

> <span data-ttu-id="9a2fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a2fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a2fe-106">Rufen Sie eine Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten auf Grundlage des Bezeichners ab.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-106">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a2fe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a2fe-107">Permissions</span></span>
<span data-ttu-id="9a2fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a2fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a2fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a2fe-110">Permission type</span></span> | <span data-ttu-id="9a2fe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a2fe-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9a2fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a2fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a2fe-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a2fe-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="9a2fe-114">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="9a2fe-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9a2fe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a2fe-115">Not supported.</span></span>|
|<span data-ttu-id="9a2fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a2fe-116">Application</span></span>| <span data-ttu-id="9a2fe-117">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a2fe-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a2fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a2fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9a2fe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a2fe-119">Request headers</span></span>
| <span data-ttu-id="9a2fe-120">Name</span><span class="sxs-lookup"><span data-stu-id="9a2fe-120">Name</span></span>       | <span data-ttu-id="9a2fe-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9a2fe-121">Type</span></span> | <span data-ttu-id="9a2fe-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a2fe-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9a2fe-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9a2fe-123">Authorization</span></span>  | <span data-ttu-id="9a2fe-124">string</span><span class="sxs-lookup"><span data-stu-id="9a2fe-124">string</span></span>  | <span data-ttu-id="9a2fe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a2fe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a2fe-127">Request body</span></span>
<span data-ttu-id="9a2fe-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9a2fe-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a2fe-129">Response</span></span>
<span data-ttu-id="9a2fe-130">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-130">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a2fe-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a2fe-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a2fe-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a2fe-132">Request</span></span>
<span data-ttu-id="9a2fe-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="9a2fe-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a2fe-134">Response</span></span>
<span data-ttu-id="9a2fe-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9a2fe-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9a2fe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2487

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/$entity",
    "displayName": "Test Profile",
    "state": "provisioned",
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
    "licensesToAssign": 
         [
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
