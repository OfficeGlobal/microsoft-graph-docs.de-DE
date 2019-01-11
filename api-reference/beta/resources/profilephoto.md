---
title: profilePhoto-Ressourcentyp
description: Ein Profilfoto von einem Benutzer, Gruppe oder ein Outlook-Kontakt auf die in Exchange Online oder Azure Active Directory (AAD) zugegriffen. Es ist nicht im Base64-codierte Binärdaten.
localization_priority: Normal
ms.openlocfilehash: 7754d70c4e59b13b1b0003022ddc0f185cc18ae2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837068"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="7dd17-104">profilePhoto-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7dd17-104">profilePhoto resource type</span></span>

> <span data-ttu-id="7dd17-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7dd17-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7dd17-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7dd17-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7dd17-107">Ein Profilfoto von einem Benutzer, Gruppe oder ein Outlook-Kontakt auf die in Exchange Online oder Azure Active Directory (AAD) zugegriffen.</span><span class="sxs-lookup"><span data-stu-id="7dd17-107">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="7dd17-108">Es ist nicht im Base64-codierte Binärdaten.</span><span class="sxs-lookup"><span data-stu-id="7dd17-108">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="7dd17-109">Die unterstützten Größen der HD-Fotos auf Exchange Online sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="7dd17-109">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="7dd17-110">Klicken Sie auf AAD können Fotos alle Dimension sein.</span><span class="sxs-lookup"><span data-stu-id="7dd17-110">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="7dd17-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="7dd17-111">Methods</span></span>

| <span data-ttu-id="7dd17-112">Methode</span><span class="sxs-lookup"><span data-stu-id="7dd17-112">Method</span></span>       | <span data-ttu-id="7dd17-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7dd17-113">Return Type</span></span>  |<span data-ttu-id="7dd17-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7dd17-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7dd17-115">profilePhoto abrufen</span><span class="sxs-lookup"><span data-stu-id="7dd17-115">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="7dd17-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="7dd17-116">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="7dd17-117">Rufen Sie die angegebenen **ProfilePhoto** oder der Metadaten (**ProfilePhoto** Eigenschaften).</span><span class="sxs-lookup"><span data-stu-id="7dd17-117">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="7dd17-118">Update</span><span class="sxs-lookup"><span data-stu-id="7dd17-118">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="7dd17-119">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="7dd17-119">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="7dd17-p105">Weist dem angegebenen Benutzer, der angegebenen Gruppe oder dem angegebenen Kontakt ein Foto zu. Das Foto sollte binär sein. Es ersetzt vorhandene Fotos (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="7dd17-p105">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="7dd17-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7dd17-123">Properties</span></span>
| <span data-ttu-id="7dd17-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7dd17-124">Property</span></span>     | <span data-ttu-id="7dd17-125">Typ</span><span class="sxs-lookup"><span data-stu-id="7dd17-125">Type</span></span>   |<span data-ttu-id="7dd17-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7dd17-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7dd17-127">id</span><span class="sxs-lookup"><span data-stu-id="7dd17-127">id</span></span>|<span data-ttu-id="7dd17-128">string</span><span class="sxs-lookup"><span data-stu-id="7dd17-128">string</span></span>|<span data-ttu-id="7dd17-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7dd17-129">Read-only.</span></span>|
|<span data-ttu-id="7dd17-130">height</span><span class="sxs-lookup"><span data-stu-id="7dd17-130">height</span></span>|<span data-ttu-id="7dd17-131">int32</span><span class="sxs-lookup"><span data-stu-id="7dd17-131">int32</span></span>|<span data-ttu-id="7dd17-p106">Die Höhe des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7dd17-p106">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="7dd17-134">width</span><span class="sxs-lookup"><span data-stu-id="7dd17-134">width</span></span>|<span data-ttu-id="7dd17-135">int32</span><span class="sxs-lookup"><span data-stu-id="7dd17-135">int32</span></span>|<span data-ttu-id="7dd17-p107">Die Breite des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7dd17-p107">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dd17-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7dd17-138">Relationships</span></span>
<span data-ttu-id="7dd17-139">Keine</span><span class="sxs-lookup"><span data-stu-id="7dd17-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7dd17-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7dd17-140">JSON representation</span></span>

<span data-ttu-id="7dd17-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7dd17-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
