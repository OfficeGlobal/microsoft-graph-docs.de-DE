---
title: Sync auf ein EducationSynchronizationProfile fortsetzen
description: Setzen Sie die Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten fort.
ms.openlocfilehash: a184c6d7903da891d93275f87501ab38f83c3e88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063082"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="a379d-103">Sync auf ein EducationSynchronizationProfile fortsetzen</span><span class="sxs-lookup"><span data-stu-id="a379d-103">Resume sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="a379d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a379d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a379d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a379d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a379d-106">Setzen Sie die Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten fort.</span><span class="sxs-lookup"><span data-stu-id="a379d-106">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a379d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a379d-107">Permissions</span></span>
<span data-ttu-id="a379d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a379d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a379d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a379d-110">Permission type</span></span> | <span data-ttu-id="a379d-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a379d-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="a379d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a379d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a379d-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a379d-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="a379d-114">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="a379d-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a379d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a379d-115">Not supported.</span></span>|
|<span data-ttu-id="a379d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a379d-116">Application</span></span>|<span data-ttu-id="a379d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a379d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a379d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a379d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="a379d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a379d-119">Request headers</span></span>
| <span data-ttu-id="a379d-120">Name</span><span class="sxs-lookup"><span data-stu-id="a379d-120">Name</span></span>       | <span data-ttu-id="a379d-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a379d-121">Type</span></span> | <span data-ttu-id="a379d-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a379d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a379d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a379d-123">Authorization</span></span>  | <span data-ttu-id="a379d-124">string</span><span class="sxs-lookup"><span data-stu-id="a379d-124">string</span></span>  | <span data-ttu-id="a379d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a379d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a379d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a379d-127">Request body</span></span>
<span data-ttu-id="a379d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a379d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a379d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a379d-129">Response</span></span>
<span data-ttu-id="a379d-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a379d-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a379d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a379d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a379d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a379d-132">Request</span></span>
<span data-ttu-id="a379d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a379d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="a379d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a379d-134">Response</span></span>

<span data-ttu-id="a379d-135">Es ist keine Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a379d-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```