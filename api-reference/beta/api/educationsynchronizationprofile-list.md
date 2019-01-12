---
title: Liste educationSynchronizationProfiles
description: Abrufen der Auflistung der Schule Daten Synchronisierungsprofile in den Mandanten an.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a51650c0ea4891ea1114d73fc9afd1fbb99ea6a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965145"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="a909c-103">Liste educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="a909c-103">List educationSynchronizationProfiles</span></span>

> <span data-ttu-id="a909c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a909c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a909c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a909c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a909c-106">Abrufen der Auflistung der Schule Daten [Profile Synchronization](../resources/educationsynchronizationprofile.md) in den Mandanten an.</span><span class="sxs-lookup"><span data-stu-id="a909c-106">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a909c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a909c-107">Permissions</span></span>
<span data-ttu-id="a909c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a909c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a909c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a909c-110">Permission type</span></span> | <span data-ttu-id="a909c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a909c-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="a909c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a909c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a909c-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a909c-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="a909c-114">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="a909c-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a909c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a909c-115">Not supported.</span></span>|
|<span data-ttu-id="a909c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a909c-116">Application</span></span>|<span data-ttu-id="a909c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a909c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a909c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a909c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a909c-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a909c-119">Optional query parameters</span></span>
<span data-ttu-id="a909c-120">Diese Methode unterstützt die folgenden [Parameter für OData-Abfrage](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen: $filter, $orderby, $top, $skip und $count.</span><span class="sxs-lookup"><span data-stu-id="a909c-120">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a909c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a909c-121">Request headers</span></span>
| <span data-ttu-id="a909c-122">Name</span><span class="sxs-lookup"><span data-stu-id="a909c-122">Name</span></span>       | <span data-ttu-id="a909c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="a909c-123">Type</span></span> | <span data-ttu-id="a909c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a909c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a909c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a909c-125">Authorization</span></span>  | <span data-ttu-id="a909c-126">string</span><span class="sxs-lookup"><span data-stu-id="a909c-126">string</span></span>  | <span data-ttu-id="a909c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a909c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a909c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a909c-129">Request body</span></span>
<span data-ttu-id="a909c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a909c-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a909c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a909c-131">Response</span></span>
<span data-ttu-id="a909c-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a909c-132">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a909c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a909c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a909c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a909c-134">Request</span></span>
<span data-ttu-id="a909c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a909c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="a909c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a909c-136">Response</span></span>
<span data-ttu-id="a909c-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a909c-137">The following is an example of the response.</span></span> 

><span data-ttu-id="a909c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a909c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
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
            "@odata.type": "#microsoft.graph.educationCsvDataProvider",
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
  ]
}
```
