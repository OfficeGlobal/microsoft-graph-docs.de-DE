---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei oder einen Ordner kopieren
ms.openlocfilehash: 6740091f887e42a14b2a42c99ee586af4254c473
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="799d6-102">DriveItem kopieren</span><span class="sxs-lookup"><span data-stu-id="799d6-102">Copy a DriveItem</span></span>

<span data-ttu-id="799d6-103">Erstellt asynchron eine Kopie eines [driveItem][item-resource] (einschließlich aller untergeordneten Elemente) unter einem neuen übergeordneten Element oder mit einem neuen Namen.</span><span class="sxs-lookup"><span data-stu-id="799d6-103">Creates a copy of a [driveItem] (including any children) under a new parent or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="799d6-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="799d6-104">Permissions</span></span>

<span data-ttu-id="799d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="799d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="799d6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="799d6-107">Permission type</span></span>      | <span data-ttu-id="799d6-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="799d6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="799d6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="799d6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="799d6-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="799d6-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="799d6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="799d6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="799d6-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="799d6-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="799d6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="799d6-113">Application</span></span> | <span data-ttu-id="799d6-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="799d6-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="799d6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="799d6-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="799d6-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="799d6-116">Request body</span></span>

<span data-ttu-id="799d6-117">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="799d6-117">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="799d6-118">Name</span><span class="sxs-lookup"><span data-stu-id="799d6-118">Name</span></span>            | <span data-ttu-id="799d6-119">Wert</span><span class="sxs-lookup"><span data-stu-id="799d6-119">Value</span></span>                                          | <span data-ttu-id="799d6-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="799d6-120">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="799d6-121">parentReference</span><span class="sxs-lookup"><span data-stu-id="799d6-121">parentReference</span></span> | [<span data-ttu-id="799d6-122">ItemReference</span><span class="sxs-lookup"><span data-stu-id="799d6-122">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="799d6-p102">Optional.  Verweis auf das übergeordnete Element, in dem die Kopie erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="799d6-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="799d6-125">name</span><span class="sxs-lookup"><span data-stu-id="799d6-125">name</span></span>            | <span data-ttu-id="799d6-126">string</span><span class="sxs-lookup"><span data-stu-id="799d6-126">string</span></span>                                         | <span data-ttu-id="799d6-p103">Optional.  Der neue Name der Kopie. Wenn dieser nicht angegeben wird, wird der gleiche Namen wie für das Original verwendet.</span><span class="sxs-lookup"><span data-stu-id="799d6-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="799d6-130">**Hinweis:** Die _parentReference_ sollte die Parameter `driveId` und `id` für den Zielordner enthalten.</span><span class="sxs-lookup"><span data-stu-id="799d6-130">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="799d6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="799d6-131">Example</span></span>

<span data-ttu-id="799d6-132">In diesem Beispiel wird eine von `{item-id}` mit einem `driveId`- und `id`-Wert identifizierte Datei in einen Ordner kopiert.</span><span class="sxs-lookup"><span data-stu-id="799d6-132">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="799d6-133">Die neue Kopie der Datei erhält den Namen `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="799d6-133">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

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

## <a name="response"></a><span data-ttu-id="799d6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="799d6-134">Response</span></span>

<span data-ttu-id="799d6-135">Die Methode gibt zusammen mit der Annahme der Anforderung Details zur [Überwachung des Fortschritts](../../../concepts/long_running_actions_overview.md) des Kopiervorgangs zurück.</span><span class="sxs-lookup"><span data-stu-id="799d6-135">Returns details about how to [monitor the progress](../../../concepts/long_running_actions_overview.md) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="799d6-136">Der Wert des `Location`-Headers enthält eine Dienst-URL, die den aktuellen Status des Kopiervorgangs zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="799d6-136">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation.</span></span>
<span data-ttu-id="799d6-137">Anhand dieser Informationen können Sie [herausfinden, wann der Kopiervorgang abgeschlossen ist](../../../concepts/long_running_actions_overview.md).</span><span class="sxs-lookup"><span data-stu-id="799d6-137">You can use this info to [determine when the copy has finished](../../../concepts/long_running_actions_overview.md).</span></span>

### <a name="remarks"></a><span data-ttu-id="799d6-138">Hinweise</span><span class="sxs-lookup"><span data-stu-id="799d6-138">Remarks</span></span>

<span data-ttu-id="799d6-p106">In vielen Fällen wird die Aktion zum Kopieren asynchron durchgeführt. Die Antwort der API gibt nur an, dass der Kopiervorgang akzeptiert oder abgelehnt wurde, wenn der Zieldateiname zum Beispiel bereits verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="799d6-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
