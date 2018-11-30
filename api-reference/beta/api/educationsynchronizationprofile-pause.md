---
title: Pause-Synchronisierung auf ein educationSynchronizationProfile
description: Halten Sie die Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten.
ms.openlocfilehash: ee2ed2133619bbcded7a31afece55191a0cfd4e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058606"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="db90a-103">Pause-Synchronisierung auf ein educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="db90a-103">Pause sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="db90a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="db90a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db90a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="db90a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db90a-106">Halten Sie die Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="db90a-106">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="db90a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db90a-107">Permissions</span></span>
<span data-ttu-id="db90a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db90a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db90a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db90a-110">Permission type</span></span> | <span data-ttu-id="db90a-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db90a-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="db90a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db90a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db90a-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db90a-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="db90a-114">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="db90a-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="db90a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db90a-115">Not supported.</span></span>|
|<span data-ttu-id="db90a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db90a-116">Application</span></span>|<span data-ttu-id="db90a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db90a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db90a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db90a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="db90a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db90a-119">Request headers</span></span>
| <span data-ttu-id="db90a-120">Name</span><span class="sxs-lookup"><span data-stu-id="db90a-120">Name</span></span>       | <span data-ttu-id="db90a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="db90a-121">Type</span></span> | <span data-ttu-id="db90a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db90a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db90a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db90a-123">Authorization</span></span>  | <span data-ttu-id="db90a-124">string</span><span class="sxs-lookup"><span data-stu-id="db90a-124">string</span></span>  | <span data-ttu-id="db90a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="db90a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db90a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db90a-127">Request body</span></span>
<span data-ttu-id="db90a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="db90a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="db90a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="db90a-129">Response</span></span>
<span data-ttu-id="db90a-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db90a-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db90a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db90a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db90a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db90a-132">Request</span></span>
<span data-ttu-id="db90a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db90a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="db90a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="db90a-134">Response</span></span>

<span data-ttu-id="db90a-135">Es ist keine Antworttext.</span><span class="sxs-lookup"><span data-stu-id="db90a-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```