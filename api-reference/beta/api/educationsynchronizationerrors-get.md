---
title: Abrufen von educationSynchronizationErrors
description: 'Rufen Sie die Fehler, die während der Validierung und/oder während der Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten. '
ms.openlocfilehash: 8d4341eafa515f79de6dda2f40f22c990ed5926c
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209663"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="ba097-103">Abrufen von educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="ba097-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="ba097-104">Rufen Sie die Fehler, die während der Validierung und/oder während der Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ba097-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ba097-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ba097-105">Permissions</span></span>
<span data-ttu-id="ba097-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba097-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba097-108">Permission type</span></span> | <span data-ttu-id="ba097-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba097-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="ba097-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba097-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba097-111">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba097-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ba097-112">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="ba097-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ba097-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba097-113">Not supported.</span></span>|
|<span data-ttu-id="ba097-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba097-114">Application</span></span>| <span data-ttu-id="ba097-115">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba097-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba097-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba097-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ba097-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ba097-117">Optional query parameters</span></span>
<span data-ttu-id="ba097-118">Diese Methode unterstützt die folgenden [Parameter für OData-Abfrage](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen: $filter, $orderby, $top, $skip und $count.</span><span class="sxs-lookup"><span data-stu-id="ba097-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba097-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba097-119">Request headers</span></span>
| <span data-ttu-id="ba097-120">Name</span><span class="sxs-lookup"><span data-stu-id="ba097-120">Name</span></span>       | <span data-ttu-id="ba097-121">Typ</span><span class="sxs-lookup"><span data-stu-id="ba097-121">Type</span></span> | <span data-ttu-id="ba097-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba097-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ba097-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba097-123">Authorization</span></span>  | <span data-ttu-id="ba097-124">string</span><span class="sxs-lookup"><span data-stu-id="ba097-124">string</span></span>  | <span data-ttu-id="ba097-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ba097-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba097-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba097-127">Request body</span></span>
<span data-ttu-id="ba097-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ba097-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ba097-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba097-129">Response</span></span>
<span data-ttu-id="ba097-130">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eine Auflistung von [Synchronisierung Error](../resources/educationsynchronizationerror.md) -Objekte in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ba097-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba097-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba097-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba097-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba097-132">Request</span></span>
<span data-ttu-id="ba097-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ba097-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```

##### <a name="response"></a><span data-ttu-id="ba097-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba097-134">Response</span></span>
<span data-ttu-id="ba097-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ba097-135">The following is an example of the response.</span></span> 

><span data-ttu-id="ba097-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ba097-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/errors",
    "@odata.count": 14,
    "value": [
        {
            "entryType": "Student",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
            "joiningValue": "richard.2wilson@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:45Z",
            "reportableIdentifier": "richard.2wilson"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "alberto2.dorsey@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "alberto2.dorsey"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "madeline2.bullock@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "madeline2.bullock"
        }
    ]
}
```
