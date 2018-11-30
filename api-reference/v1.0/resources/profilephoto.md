---
title: profilePhoto-Ressourcentyp
description: Ein Profilfoto eines Benutzers, einer Gruppe oder eines Outlook-Kontakts, auf den bzw. die von Exchange Online zugegriffen wird. Es handelt sich um Binärdaten, die nicht in Base-64 codiert sind.
ms.openlocfilehash: c5f74e1dcd48e42a2e17d5a64e6ed4b9e9cca5e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019997"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="3e427-104">profilePhoto-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3e427-104">profilePhoto resource type</span></span>
<span data-ttu-id="3e427-p102">Ein Profilfoto eines Benutzers, einer Gruppe oder eines Outlook-Kontakts, auf den bzw. die von Exchange Online zugegriffen wird. Es handelt sich um Binärdaten, die nicht in Base-64 codiert sind.</span><span class="sxs-lookup"><span data-stu-id="3e427-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="3e427-107">Die unterstützten Größen der HD-Fotos auf Exchange Online sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="3e427-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="3e427-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="3e427-108">Methods</span></span>

| <span data-ttu-id="3e427-109">Methode</span><span class="sxs-lookup"><span data-stu-id="3e427-109">Method</span></span>       | <span data-ttu-id="3e427-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3e427-110">Return Type</span></span>  |<span data-ttu-id="3e427-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e427-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3e427-112">profilePhoto abrufen</span><span class="sxs-lookup"><span data-stu-id="3e427-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="3e427-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="3e427-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="3e427-114">Ruft das angegebene **profilePhoto** oder seine Metadaten (profilePhoto-Eigenschaften) ab.</span><span class="sxs-lookup"><span data-stu-id="3e427-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="3e427-115">Update</span><span class="sxs-lookup"><span data-stu-id="3e427-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="3e427-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="3e427-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="3e427-p103">Weist dem angegebenen Benutzer, der angegebenen Gruppe oder dem angegebenen Kontakt ein Foto zu. Das Foto sollte binär sein. Es ersetzt vorhandene Fotos (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="3e427-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e427-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3e427-120">Properties</span></span>
| <span data-ttu-id="3e427-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e427-121">Property</span></span>     | <span data-ttu-id="3e427-122">Typ</span><span class="sxs-lookup"><span data-stu-id="3e427-122">Type</span></span>   |<span data-ttu-id="3e427-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e427-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e427-124">id</span><span class="sxs-lookup"><span data-stu-id="3e427-124">id</span></span>|<span data-ttu-id="3e427-125">string</span><span class="sxs-lookup"><span data-stu-id="3e427-125">string</span></span>|<span data-ttu-id="3e427-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3e427-126">Read-only.</span></span>|
|<span data-ttu-id="3e427-127">height</span><span class="sxs-lookup"><span data-stu-id="3e427-127">height</span></span>|<span data-ttu-id="3e427-128">int32</span><span class="sxs-lookup"><span data-stu-id="3e427-128">int32</span></span>|<span data-ttu-id="3e427-p104">Die Höhe des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3e427-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="3e427-131">width</span><span class="sxs-lookup"><span data-stu-id="3e427-131">width</span></span>|<span data-ttu-id="3e427-132">int32</span><span class="sxs-lookup"><span data-stu-id="3e427-132">int32</span></span>|<span data-ttu-id="3e427-p105">Die Breite des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3e427-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e427-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3e427-135">Relationships</span></span>
<span data-ttu-id="3e427-136">Keine</span><span class="sxs-lookup"><span data-stu-id="3e427-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3e427-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3e427-137">JSON representation</span></span>

<span data-ttu-id="3e427-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3e427-138">Here is a JSON representation of the resource.</span></span>

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
