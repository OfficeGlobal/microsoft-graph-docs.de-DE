---
title: Löschen einer educationSynchronizationProfile
description: Löschen Sie eine Schule Synchronisierung Datenprofil im Mandanten auf Grundlage des Bezeichners.
ms.openlocfilehash: 829b723b48eb9a15750bc9d0e00ba50d432e8ab6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062774"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="40e44-103">Löschen einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="40e44-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="40e44-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40e44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40e44-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40e44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40e44-106">Löschen eines Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten auf Grundlage des Bezeichners.</span><span class="sxs-lookup"><span data-stu-id="40e44-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="40e44-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="40e44-107">Permissions</span></span>
<span data-ttu-id="40e44-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40e44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40e44-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40e44-110">Permission type</span></span> | <span data-ttu-id="40e44-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="40e44-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="40e44-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40e44-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40e44-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40e44-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="40e44-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40e44-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40e44-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40e44-115">Request headers</span></span>
| <span data-ttu-id="40e44-116">Name</span><span class="sxs-lookup"><span data-stu-id="40e44-116">Name</span></span>       | <span data-ttu-id="40e44-117">Typ</span><span class="sxs-lookup"><span data-stu-id="40e44-117">Type</span></span> | <span data-ttu-id="40e44-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40e44-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="40e44-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="40e44-119">Authorization</span></span>  | <span data-ttu-id="40e44-120">string</span><span class="sxs-lookup"><span data-stu-id="40e44-120">string</span></span>  | <span data-ttu-id="40e44-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="40e44-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="40e44-123">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="40e44-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="40e44-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40e44-124">Not supported.</span></span>|
|<span data-ttu-id="40e44-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40e44-125">Application</span></span>|<span data-ttu-id="40e44-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40e44-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40e44-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40e44-127">Request body</span></span>
<span data-ttu-id="40e44-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="40e44-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="40e44-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="40e44-129">Response</span></span>
<span data-ttu-id="40e44-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben, aber kein Antworttext.</span><span class="sxs-lookup"><span data-stu-id="40e44-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="40e44-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40e44-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40e44-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40e44-132">Request</span></span>
<span data-ttu-id="40e44-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40e44-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="40e44-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="40e44-134">Response</span></span>
<span data-ttu-id="40e44-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40e44-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
