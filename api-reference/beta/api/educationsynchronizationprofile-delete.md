---
title: Löschen einer educationSynchronizationProfile
description: Löschen Sie eine Schule Synchronisierung Datenprofil im Mandanten auf Grundlage des Bezeichners.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d3c55cd90734fa78654baf10c940cd0debc57c50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976156"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="53ebf-103">Löschen einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="53ebf-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="53ebf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53ebf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53ebf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53ebf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53ebf-106">Löschen eines Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten auf Grundlage des Bezeichners.</span><span class="sxs-lookup"><span data-stu-id="53ebf-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="53ebf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53ebf-107">Permissions</span></span>
<span data-ttu-id="53ebf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53ebf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53ebf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53ebf-110">Permission type</span></span> | <span data-ttu-id="53ebf-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53ebf-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="53ebf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53ebf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53ebf-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53ebf-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="53ebf-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53ebf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="53ebf-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53ebf-115">Request headers</span></span>
| <span data-ttu-id="53ebf-116">Name</span><span class="sxs-lookup"><span data-stu-id="53ebf-116">Name</span></span>       | <span data-ttu-id="53ebf-117">Typ</span><span class="sxs-lookup"><span data-stu-id="53ebf-117">Type</span></span> | <span data-ttu-id="53ebf-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53ebf-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53ebf-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="53ebf-119">Authorization</span></span>  | <span data-ttu-id="53ebf-120">string</span><span class="sxs-lookup"><span data-stu-id="53ebf-120">string</span></span>  | <span data-ttu-id="53ebf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53ebf-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="53ebf-123">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="53ebf-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="53ebf-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53ebf-124">Not supported.</span></span>|
|<span data-ttu-id="53ebf-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53ebf-125">Application</span></span>|<span data-ttu-id="53ebf-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53ebf-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53ebf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53ebf-127">Request body</span></span>
<span data-ttu-id="53ebf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="53ebf-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53ebf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="53ebf-129">Response</span></span>
<span data-ttu-id="53ebf-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben, aber kein Antworttext.</span><span class="sxs-lookup"><span data-stu-id="53ebf-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="53ebf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53ebf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53ebf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53ebf-132">Request</span></span>
<span data-ttu-id="53ebf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53ebf-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="53ebf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="53ebf-134">Response</span></span>
<span data-ttu-id="53ebf-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53ebf-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
