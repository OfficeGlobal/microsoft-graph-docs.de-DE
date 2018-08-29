---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ItemReference
ms.openlocfilehash: e83b0a18725d587094a00e9cc84a51b030d83340
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268466"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="c1a86-102">ItemReference-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c1a86-102">ItemReference resource type</span></span>

<span data-ttu-id="c1a86-103">Die **ItemReference**-Ressource enthält Informationen, die erforderlich sind, um ein [DriveItem](driveitem.md) über die API zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="c1a86-103">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1a86-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c1a86-104">JSON representation</span></span>

<span data-ttu-id="c1a86-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c1a86-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="c1a86-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c1a86-106">Properties</span></span>

| <span data-ttu-id="c1a86-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1a86-107">Property</span></span>      | <span data-ttu-id="c1a86-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c1a86-108">Type</span></span>              | <span data-ttu-id="c1a86-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1a86-109">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="c1a86-110">driveId</span><span class="sxs-lookup"><span data-stu-id="c1a86-110">driveId</span></span>       | <span data-ttu-id="c1a86-111">String</span><span class="sxs-lookup"><span data-stu-id="c1a86-111">String</span></span>            | <span data-ttu-id="c1a86-p101">Eindeutiger Bezeichner der drive-Instanz, die das Element enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c1a86-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="c1a86-114">driveType</span><span class="sxs-lookup"><span data-stu-id="c1a86-114">driveType</span></span>     | <span data-ttu-id="c1a86-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1a86-115">String</span></span>            | <span data-ttu-id="c1a86-116">Identifiziert den Laufwerkstyp.</span><span class="sxs-lookup"><span data-stu-id="c1a86-116">Identifies the type of drive.</span></span> <span data-ttu-id="c1a86-117">Werte finden Sie unter [drive][]-Ressource.</span><span class="sxs-lookup"><span data-stu-id="c1a86-117">See [drive][] resource for values.</span></span>
| <span data-ttu-id="c1a86-118">id</span><span class="sxs-lookup"><span data-stu-id="c1a86-118">id</span></span>            | <span data-ttu-id="c1a86-119">String</span><span class="sxs-lookup"><span data-stu-id="c1a86-119">String</span></span>            | <span data-ttu-id="c1a86-p103">Eindeutiger Bezeichner des Elements im Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c1a86-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="c1a86-122">name</span><span class="sxs-lookup"><span data-stu-id="c1a86-122">name</span></span>          | <span data-ttu-id="c1a86-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1a86-123">String</span></span>            | <span data-ttu-id="c1a86-p104">Der Name des Elements, auf das verwiesen wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c1a86-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="c1a86-126">Pfad</span><span class="sxs-lookup"><span data-stu-id="c1a86-126">path</span></span>          | <span data-ttu-id="c1a86-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1a86-127">String</span></span>            | <span data-ttu-id="c1a86-p105">Pfad, der verwendet werden kann, um zu dem Element zu navigieren. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c1a86-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="c1a86-130">shareId</span><span class="sxs-lookup"><span data-stu-id="c1a86-130">shareId</span></span>       | <span data-ttu-id="c1a86-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1a86-131">String</span></span>            | <span data-ttu-id="c1a86-132">Ein eindeutiger Bezeichner für eine freigegebene Ressource, auf die über [Freigabe][]-API zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="c1a86-132">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="c1a86-133">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="c1a86-133">sharepointIds</span></span> | <span data-ttu-id="c1a86-134">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="c1a86-134">[sharepointIds][]</span></span> | <span data-ttu-id="c1a86-p106">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c1a86-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Freigabe]: ../api/shares_get.md
[Shares]: ../api/shares_get.md

## <a name="remarks"></a><span data-ttu-id="c1a86-140">Hinweise</span><span class="sxs-lookup"><span data-stu-id="c1a86-140">Remarks</span></span>

<span data-ttu-id="c1a86-141">Um ein **driveItem**-Element aus einer **itemReference**-Ressource zu adressieren, erstellen Sie eine URL im folgenden Format:</span><span class="sxs-lookup"><span data-stu-id="c1a86-141">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="c1a86-142">Der **path**-Wert ist ein API-Pfad relativ zu dem Ziellaufwerk, z. B.: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="c1a86-142">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="c1a86-143">Um den lesbaren Pfad für ein Breadcrumb abzurufen, können Sie alles bis zum ersten `:` in der Pfadzeichenfolge problemlos ignorieren.</span><span class="sxs-lookup"><span data-stu-id="c1a86-143">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/itemreference.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ItemReference"
} -->
