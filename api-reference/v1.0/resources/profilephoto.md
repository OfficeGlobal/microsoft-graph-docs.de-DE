---
title: profilePhoto-Ressourcentyp
description: Ein Profilfoto eines Benutzers, einer Gruppe oder eines Outlook-Kontakts, auf den bzw. die von Exchange Online zugegriffen wird. Es handelt sich um Binärdaten, die nicht in Base-64 codiert sind.
localization_priority: Priority
ms.openlocfilehash: b1901928a97356b2a9808a446d34981fd74bf456
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876566"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="ad9ed-104">profilePhoto-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ad9ed-104">profilePhoto resource type</span></span>
<span data-ttu-id="ad9ed-p102">Ein Profilfoto eines Benutzers, einer Gruppe oder eines Outlook-Kontakts, auf den bzw. die von Exchange Online zugegriffen wird. Es handelt sich um Binärdaten, die nicht in Base-64 codiert sind.</span><span class="sxs-lookup"><span data-stu-id="ad9ed-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="ad9ed-107">Die unterstützten Größen der HD-Fotos auf Exchange Online sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="ad9ed-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="ad9ed-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="ad9ed-108">Methods</span></span>

| <span data-ttu-id="ad9ed-109">Methode</span><span class="sxs-lookup"><span data-stu-id="ad9ed-109">Method</span></span>       | <span data-ttu-id="ad9ed-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ad9ed-110">Return Type</span></span>  |<span data-ttu-id="ad9ed-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad9ed-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad9ed-112">profilePhoto abrufen</span><span class="sxs-lookup"><span data-stu-id="ad9ed-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="ad9ed-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ad9ed-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="ad9ed-114">Ruft das angegebene **profilePhoto** oder seine Metadaten (profilePhoto-Eigenschaften) ab.</span><span class="sxs-lookup"><span data-stu-id="ad9ed-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="ad9ed-115">Update</span><span class="sxs-lookup"><span data-stu-id="ad9ed-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="ad9ed-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ad9ed-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="ad9ed-p103">Weist dem angegebenen Benutzer, der angegebenen Gruppe oder dem angegebenen Kontakt ein Foto zu. Das Foto sollte binär sein. Es ersetzt vorhandene Fotos (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="ad9ed-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad9ed-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad9ed-120">Properties</span></span>
| <span data-ttu-id="ad9ed-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad9ed-121">Property</span></span>     | <span data-ttu-id="ad9ed-122">Typ</span><span class="sxs-lookup"><span data-stu-id="ad9ed-122">Type</span></span>   |<span data-ttu-id="ad9ed-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad9ed-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad9ed-124">id</span><span class="sxs-lookup"><span data-stu-id="ad9ed-124">id</span></span>|<span data-ttu-id="ad9ed-125">string</span><span class="sxs-lookup"><span data-stu-id="ad9ed-125">string</span></span>|<span data-ttu-id="ad9ed-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ad9ed-126">Read-only.</span></span>|
|<span data-ttu-id="ad9ed-127">height</span><span class="sxs-lookup"><span data-stu-id="ad9ed-127">height</span></span>|<span data-ttu-id="ad9ed-128">int32</span><span class="sxs-lookup"><span data-stu-id="ad9ed-128">int32</span></span>|<span data-ttu-id="ad9ed-p104">Die Höhe des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ad9ed-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="ad9ed-131">width</span><span class="sxs-lookup"><span data-stu-id="ad9ed-131">width</span></span>|<span data-ttu-id="ad9ed-132">int32</span><span class="sxs-lookup"><span data-stu-id="ad9ed-132">int32</span></span>|<span data-ttu-id="ad9ed-p105">Die Breite des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ad9ed-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad9ed-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ad9ed-135">Relationships</span></span>
<span data-ttu-id="ad9ed-136">Keine</span><span class="sxs-lookup"><span data-stu-id="ad9ed-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ad9ed-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad9ed-137">JSON representation</span></span>

<span data-ttu-id="ad9ed-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad9ed-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
