---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei oder einen Ordner kopieren
localization_priority: Normal
ms.openlocfilehash: b1d949d7a0bb19d03feccf353ec4803c37e7ec7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828070"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="0027f-102">DriveItem kopieren</span><span class="sxs-lookup"><span data-stu-id="0027f-102">Copy a DriveItem</span></span>

<span data-ttu-id="0027f-103">Erstellt asynchron eine Kopie eines [driveItem][item-resource] (einschließlich aller untergeordneten Elemente) unter einem neuen übergeordneten Element oder mit einem neuen Namen.</span><span class="sxs-lookup"><span data-stu-id="0027f-103">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="0027f-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0027f-104">Permissions</span></span>

<span data-ttu-id="0027f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0027f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0027f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0027f-107">Permission type</span></span>      | <span data-ttu-id="0027f-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0027f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0027f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0027f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0027f-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0027f-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0027f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0027f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0027f-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0027f-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0027f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0027f-113">Application</span></span> | <span data-ttu-id="0027f-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0027f-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0027f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0027f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="0027f-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0027f-116">Request body</span></span>

<span data-ttu-id="0027f-117">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0027f-117">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="0027f-118">Name</span><span class="sxs-lookup"><span data-stu-id="0027f-118">Name</span></span>            | <span data-ttu-id="0027f-119">Wert</span><span class="sxs-lookup"><span data-stu-id="0027f-119">Value</span></span>                                          | <span data-ttu-id="0027f-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0027f-120">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0027f-121">parentReference</span><span class="sxs-lookup"><span data-stu-id="0027f-121">parentReference</span></span> | [<span data-ttu-id="0027f-122">ItemReference</span><span class="sxs-lookup"><span data-stu-id="0027f-122">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="0027f-p102">Optional.  Verweis auf das übergeordnete Element, in dem die Kopie erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="0027f-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="0027f-125">name</span><span class="sxs-lookup"><span data-stu-id="0027f-125">name</span></span>            | <span data-ttu-id="0027f-126">string</span><span class="sxs-lookup"><span data-stu-id="0027f-126">string</span></span>                                         | <span data-ttu-id="0027f-p103">Optional.  Der neue Name der Kopie. Wenn dieser nicht angegeben wird, wird der gleiche Namen wie für das Original verwendet.</span><span class="sxs-lookup"><span data-stu-id="0027f-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="0027f-130">**Hinweis:** Die _ParentReference_ sollte die Parameter `driveId` und `id` für den Zielordner enthalten.</span><span class="sxs-lookup"><span data-stu-id="0027f-130">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="0027f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0027f-131">Example</span></span>

<span data-ttu-id="0027f-132">In diesem Beispiel wird eine von `{item-id}` mit einem `driveId`- und `id`-Wert identifizierte Datei in einen Ordner kopiert.</span><span class="sxs-lookup"><span data-stu-id="0027f-132">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="0027f-133">Die neue Kopie der Datei erhält den Namen `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="0027f-133">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "tags": "service.graph", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```

## <a name="response"></a><span data-ttu-id="0027f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0027f-134">Response</span></span>

<span data-ttu-id="0027f-135">Die Methode gibt zusammen mit der Annahme der Anforderung Details zur [Überwachung des Fortschritts](/graph/long-running-actions-overview) des Kopiervorgangs zurück.</span><span class="sxs-lookup"><span data-stu-id="0027f-135">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="0027f-136">Der Wert des `Location`-Headers enthält eine Dienst-URL, die den aktuellen Status des Kopiervorgangs zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="0027f-136">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation.</span></span>
<span data-ttu-id="0027f-137">Anhand dieser Informationen können Sie [herausfinden, wann der Kopiervorgang abgeschlossen ist](/graph/long-running-actions-overview).</span><span class="sxs-lookup"><span data-stu-id="0027f-137">You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="0027f-138">Hinweise</span><span class="sxs-lookup"><span data-stu-id="0027f-138">Remarks</span></span>

<span data-ttu-id="0027f-p106">In vielen Fällen wird die Aktion zum Kopieren asynchron durchgeführt. Die Antwort der API gibt nur an, dass der Kopiervorgang akzeptiert oder abgelehnt wurde, wenn der Zieldateiname zum Beispiel bereits verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0027f-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
