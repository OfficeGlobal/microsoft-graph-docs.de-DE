---
title: Erstellen oder Ersetzen einer historyItem
description: Erstellen Sie ein neues oder Ersetzen Sie vorhandenes Verlaufselement für einen vorhandenen Benutzeraktivität.
localization_priority: Normal
ms.openlocfilehash: 008e4bc8470ffddce4f60f71bdff68ca13ad39c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807889"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="3daa9-103">Erstellen oder Ersetzen einer historyItem</span><span class="sxs-lookup"><span data-stu-id="3daa9-103">Create or replace a historyItem</span></span>

> <span data-ttu-id="3daa9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3daa9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3daa9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3daa9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3daa9-106">Erstellen Sie ein neues oder Ersetzen Sie vorhandenes Verlaufselement für einen vorhandenen Benutzeraktivität.</span><span class="sxs-lookup"><span data-stu-id="3daa9-106">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="3daa9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3daa9-107">Permissions</span></span>

<span data-ttu-id="3daa9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3daa9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3daa9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3daa9-110">Permission type</span></span>      | <span data-ttu-id="3daa9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3daa9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3daa9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3daa9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3daa9-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="3daa9-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="3daa9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3daa9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3daa9-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="3daa9-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="3daa9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3daa9-116">Application</span></span> | <span data-ttu-id="3daa9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3daa9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3daa9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3daa9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="3daa9-119">ID muss eine GUID sein.</span><span class="sxs-lookup"><span data-stu-id="3daa9-119">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3daa9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3daa9-120">Request headers</span></span>

|<span data-ttu-id="3daa9-121">Name</span><span class="sxs-lookup"><span data-stu-id="3daa9-121">Name</span></span> | <span data-ttu-id="3daa9-122">Typ</span><span class="sxs-lookup"><span data-stu-id="3daa9-122">Type</span></span> | <span data-ttu-id="3daa9-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3daa9-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="3daa9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3daa9-124">Authorization</span></span> | <span data-ttu-id="3daa9-125">string</span><span class="sxs-lookup"><span data-stu-id="3daa9-125">string</span></span> | <span data-ttu-id="3daa9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3daa9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3daa9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3daa9-128">Request body</span></span>

<span data-ttu-id="3daa9-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [HistoryItem](../resources/projectrome-historyitem.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3daa9-129">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3daa9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3daa9-130">Response</span></span>

<span data-ttu-id="3daa9-131">Wenn der Vorgang erfolgreich war, gibt diese Methode die `201 Created` Antwortcode, wenn die HistoryItem erstellt wurde oder `200 OK` , wenn die HistoryItem ersetzt wurde.</span><span class="sxs-lookup"><span data-stu-id="3daa9-131">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="3daa9-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3daa9-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3daa9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3daa9-133">Request</span></span>

<span data-ttu-id="3daa9-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3daa9-134">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="3daa9-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3daa9-135">Response</span></span>

<span data-ttu-id="3daa9-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3daa9-136">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.historyItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
