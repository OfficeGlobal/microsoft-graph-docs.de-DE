---
title: Abrufen des Status eines educationSynchronizationProfile
description: Rufen Sie den Status eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten. Die Antwort wird den Status der auszuführenden Synchronisierung hingewiesen.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6a2d3dffd715d78bb96794808da39255db0164b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510197"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="f60d2-104">Abrufen des Status eines educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="f60d2-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f60d2-105">Rufen Sie den Status eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f60d2-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="f60d2-106">Die Antwort wird den Status der auszuführenden Synchronisierung hingewiesen.</span><span class="sxs-lookup"><span data-stu-id="f60d2-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="f60d2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f60d2-107">Permissions</span></span>
<span data-ttu-id="f60d2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f60d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f60d2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f60d2-110">Permission type</span></span> | <span data-ttu-id="f60d2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f60d2-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f60d2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f60d2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f60d2-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f60d2-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f60d2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f60d2-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f60d2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f60d2-115">Not supported.</span></span>|
|<span data-ttu-id="f60d2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f60d2-116">Application</span></span>| <span data-ttu-id="f60d2-117">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f60d2-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f60d2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f60d2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="f60d2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f60d2-119">Request headers</span></span>
| <span data-ttu-id="f60d2-120">Name</span><span class="sxs-lookup"><span data-stu-id="f60d2-120">Name</span></span>       | <span data-ttu-id="f60d2-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f60d2-121">Type</span></span> | <span data-ttu-id="f60d2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f60d2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f60d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f60d2-123">Authorization</span></span>  | <span data-ttu-id="f60d2-124">string</span><span class="sxs-lookup"><span data-stu-id="f60d2-124">string</span></span>  | <span data-ttu-id="f60d2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f60d2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f60d2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f60d2-127">Request body</span></span>
<span data-ttu-id="f60d2-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f60d2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f60d2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f60d2-129">Response</span></span>
<span data-ttu-id="f60d2-130">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [Educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f60d2-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f60d2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f60d2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f60d2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f60d2-132">Request</span></span>
<span data-ttu-id="f60d2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f60d2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="f60d2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f60d2-134">Response</span></span>
<span data-ttu-id="f60d2-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f60d2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f60d2-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f60d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
