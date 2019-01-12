---
title: Pause-Synchronisierung auf ein educationSynchronizationProfile
description: Halten Sie die Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4979ed19c9a01d6a7ff2d43f7f3755d03b4b070c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950683"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="3adb9-103">Pause-Synchronisierung auf ein educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="3adb9-103">Pause sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="3adb9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3adb9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3adb9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3adb9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3adb9-106">Halten Sie die Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3adb9-106">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="3adb9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3adb9-107">Permissions</span></span>
<span data-ttu-id="3adb9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3adb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3adb9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3adb9-110">Permission type</span></span> | <span data-ttu-id="3adb9-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3adb9-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3adb9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3adb9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3adb9-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3adb9-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="3adb9-114">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="3adb9-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3adb9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3adb9-115">Not supported.</span></span>|
|<span data-ttu-id="3adb9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3adb9-116">Application</span></span>|<span data-ttu-id="3adb9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3adb9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3adb9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3adb9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="3adb9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3adb9-119">Request headers</span></span>
| <span data-ttu-id="3adb9-120">Name</span><span class="sxs-lookup"><span data-stu-id="3adb9-120">Name</span></span>       | <span data-ttu-id="3adb9-121">Typ</span><span class="sxs-lookup"><span data-stu-id="3adb9-121">Type</span></span> | <span data-ttu-id="3adb9-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3adb9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3adb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3adb9-123">Authorization</span></span>  | <span data-ttu-id="3adb9-124">string</span><span class="sxs-lookup"><span data-stu-id="3adb9-124">string</span></span>  | <span data-ttu-id="3adb9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3adb9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3adb9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3adb9-127">Request body</span></span>
<span data-ttu-id="3adb9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3adb9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3adb9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3adb9-129">Response</span></span>
<span data-ttu-id="3adb9-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3adb9-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3adb9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3adb9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3adb9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3adb9-132">Request</span></span>
<span data-ttu-id="3adb9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3adb9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="3adb9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3adb9-134">Response</span></span>

<span data-ttu-id="3adb9-135">Es ist keine Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3adb9-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
