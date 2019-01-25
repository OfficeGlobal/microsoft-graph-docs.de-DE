---
title: Pause-Synchronisierung auf ein educationSynchronizationProfile
description: Halten Sie die Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c9ba7d2ab3f67880105d45d9d98506b8e8caaac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510932"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="e0670-103">Pause-Synchronisierung auf ein educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="e0670-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0670-104">Halten Sie die Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e0670-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0670-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0670-105">Permissions</span></span>
<span data-ttu-id="e0670-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0670-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0670-108">Permission type</span></span> | <span data-ttu-id="e0670-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0670-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e0670-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0670-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0670-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0670-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e0670-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0670-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e0670-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0670-113">Not supported.</span></span>|
|<span data-ttu-id="e0670-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0670-114">Application</span></span>|<span data-ttu-id="e0670-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0670-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0670-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0670-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="e0670-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0670-117">Request headers</span></span>
| <span data-ttu-id="e0670-118">Name</span><span class="sxs-lookup"><span data-stu-id="e0670-118">Name</span></span>       | <span data-ttu-id="e0670-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e0670-119">Type</span></span> | <span data-ttu-id="e0670-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0670-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0670-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0670-121">Authorization</span></span>  | <span data-ttu-id="e0670-122">string</span><span class="sxs-lookup"><span data-stu-id="e0670-122">string</span></span>  | <span data-ttu-id="e0670-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0670-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0670-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0670-125">Request body</span></span>
<span data-ttu-id="e0670-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e0670-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e0670-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0670-127">Response</span></span>
<span data-ttu-id="e0670-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0670-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e0670-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0670-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0670-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0670-130">Request</span></span>
<span data-ttu-id="e0670-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0670-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="e0670-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0670-132">Response</span></span>

<span data-ttu-id="e0670-133">Es ist keine Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e0670-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
