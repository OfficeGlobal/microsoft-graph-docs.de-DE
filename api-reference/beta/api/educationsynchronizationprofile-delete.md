---
title: Löschen einer educationSynchronizationProfile
description: Löschen Sie eine Schule Synchronisierung Datenprofil im Mandanten auf Grundlage des Bezeichners.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2aaa0d47bcc98c814ad525deb781ac7a7df28d87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512472"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="f33e0-103">Löschen einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="f33e0-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f33e0-104">Löschen eines Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten auf Grundlage des Bezeichners.</span><span class="sxs-lookup"><span data-stu-id="f33e0-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="f33e0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f33e0-105">Permissions</span></span>
<span data-ttu-id="f33e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f33e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f33e0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f33e0-108">Permission type</span></span> | <span data-ttu-id="f33e0-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f33e0-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f33e0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f33e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f33e0-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f33e0-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f33e0-112">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f33e0-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f33e0-113">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f33e0-113">Request headers</span></span>
| <span data-ttu-id="f33e0-114">Name</span><span class="sxs-lookup"><span data-stu-id="f33e0-114">Name</span></span>       | <span data-ttu-id="f33e0-115">Typ</span><span class="sxs-lookup"><span data-stu-id="f33e0-115">Type</span></span> | <span data-ttu-id="f33e0-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f33e0-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f33e0-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="f33e0-117">Authorization</span></span>  | <span data-ttu-id="f33e0-118">string</span><span class="sxs-lookup"><span data-stu-id="f33e0-118">string</span></span>  | <span data-ttu-id="f33e0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f33e0-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="f33e0-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f33e0-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f33e0-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f33e0-122">Not supported.</span></span>|
|<span data-ttu-id="f33e0-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f33e0-123">Application</span></span>|<span data-ttu-id="f33e0-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f33e0-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f33e0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f33e0-125">Request body</span></span>
<span data-ttu-id="f33e0-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f33e0-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f33e0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f33e0-127">Response</span></span>
<span data-ttu-id="f33e0-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben, aber kein Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f33e0-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="f33e0-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f33e0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f33e0-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f33e0-130">Request</span></span>
<span data-ttu-id="f33e0-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f33e0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="f33e0-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f33e0-132">Response</span></span>
<span data-ttu-id="f33e0-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f33e0-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
