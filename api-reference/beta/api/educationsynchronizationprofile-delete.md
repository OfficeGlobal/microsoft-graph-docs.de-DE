---
title: Löschen einer educationSynchronizationProfile
description: Löschen Sie eine Schule Synchronisierung Datenprofil im Mandanten auf Grundlage des Bezeichners.
author: mmast-msft
ms.openlocfilehash: b0287133d579915279e0f9a02bf49dd981ccf419
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343302"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="2ab4e-103">Löschen einer educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="2ab4e-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="2ab4e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2ab4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ab4e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ab4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ab4e-106">Löschen eines Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten auf Grundlage des Bezeichners.</span><span class="sxs-lookup"><span data-stu-id="2ab4e-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ab4e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2ab4e-107">Permissions</span></span>
<span data-ttu-id="2ab4e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ab4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ab4e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ab4e-110">Permission type</span></span> | <span data-ttu-id="2ab4e-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2ab4e-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2ab4e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ab4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ab4e-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ab4e-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ab4e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ab4e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2ab4e-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ab4e-115">Request headers</span></span>
| <span data-ttu-id="2ab4e-116">Name</span><span class="sxs-lookup"><span data-stu-id="2ab4e-116">Name</span></span>       | <span data-ttu-id="2ab4e-117">Typ</span><span class="sxs-lookup"><span data-stu-id="2ab4e-117">Type</span></span> | <span data-ttu-id="2ab4e-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ab4e-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2ab4e-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2ab4e-119">Authorization</span></span>  | <span data-ttu-id="2ab4e-120">string</span><span class="sxs-lookup"><span data-stu-id="2ab4e-120">string</span></span>  | <span data-ttu-id="2ab4e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2ab4e-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="2ab4e-123">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="2ab4e-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2ab4e-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ab4e-124">Not supported.</span></span>|
|<span data-ttu-id="2ab4e-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ab4e-125">Application</span></span>|<span data-ttu-id="2ab4e-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ab4e-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab4e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ab4e-127">Request body</span></span>
<span data-ttu-id="2ab4e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2ab4e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2ab4e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ab4e-129">Response</span></span>
<span data-ttu-id="2ab4e-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben, aber kein Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2ab4e-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab4e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ab4e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ab4e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ab4e-132">Request</span></span>
<span data-ttu-id="2ab4e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2ab4e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="2ab4e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ab4e-134">Response</span></span>
<span data-ttu-id="2ab4e-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2ab4e-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
