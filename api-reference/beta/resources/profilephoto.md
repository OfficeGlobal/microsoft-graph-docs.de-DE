---
title: profilePhoto-Ressourcentyp
description: Ein Profilfoto von einem Benutzer, Gruppe oder ein Outlook-Kontakt auf die in Exchange Online oder Azure Active Directory (AAD) zugegriffen. Es ist nicht im Base64-codierte Binärdaten.
localization_priority: Normal
ms.openlocfilehash: 2a831abd098fb9a0dfa95f6d6dd3a9cd5de128cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513655"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="219e0-104">profilePhoto-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="219e0-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="219e0-105">Ein Profilfoto von einem Benutzer, Gruppe oder ein Outlook-Kontakt auf die in Exchange Online oder Azure Active Directory (AAD) zugegriffen.</span><span class="sxs-lookup"><span data-stu-id="219e0-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="219e0-106">Es ist nicht im Base64-codierte Binärdaten.</span><span class="sxs-lookup"><span data-stu-id="219e0-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="219e0-107">Die unterstützten Größen der HD-Fotos auf Exchange Online sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="219e0-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="219e0-108">Klicken Sie auf AAD können Fotos alle Dimension sein.</span><span class="sxs-lookup"><span data-stu-id="219e0-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="219e0-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="219e0-109">Methods</span></span>

| <span data-ttu-id="219e0-110">Methode</span><span class="sxs-lookup"><span data-stu-id="219e0-110">Method</span></span>       | <span data-ttu-id="219e0-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="219e0-111">Return Type</span></span>  |<span data-ttu-id="219e0-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="219e0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="219e0-113">profilePhoto abrufen</span><span class="sxs-lookup"><span data-stu-id="219e0-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="219e0-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="219e0-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="219e0-115">Rufen Sie die angegebenen **ProfilePhoto** oder der Metadaten (**ProfilePhoto** Eigenschaften).</span><span class="sxs-lookup"><span data-stu-id="219e0-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="219e0-116">Update</span><span class="sxs-lookup"><span data-stu-id="219e0-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="219e0-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="219e0-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="219e0-p104">Weist dem angegebenen Benutzer, der angegebenen Gruppe oder dem angegebenen Kontakt ein Foto zu. Das Foto sollte binär sein. Es ersetzt vorhandene Fotos (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="219e0-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="219e0-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="219e0-121">Properties</span></span>
| <span data-ttu-id="219e0-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="219e0-122">Property</span></span>     | <span data-ttu-id="219e0-123">Typ</span><span class="sxs-lookup"><span data-stu-id="219e0-123">Type</span></span>   |<span data-ttu-id="219e0-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="219e0-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="219e0-125">id</span><span class="sxs-lookup"><span data-stu-id="219e0-125">id</span></span>|<span data-ttu-id="219e0-126">string</span><span class="sxs-lookup"><span data-stu-id="219e0-126">string</span></span>|<span data-ttu-id="219e0-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="219e0-127">Read-only.</span></span>|
|<span data-ttu-id="219e0-128">height</span><span class="sxs-lookup"><span data-stu-id="219e0-128">height</span></span>|<span data-ttu-id="219e0-129">int32</span><span class="sxs-lookup"><span data-stu-id="219e0-129">int32</span></span>|<span data-ttu-id="219e0-p105">Die Höhe des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="219e0-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="219e0-132">width</span><span class="sxs-lookup"><span data-stu-id="219e0-132">width</span></span>|<span data-ttu-id="219e0-133">int32</span><span class="sxs-lookup"><span data-stu-id="219e0-133">int32</span></span>|<span data-ttu-id="219e0-p106">Die Breite des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="219e0-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="219e0-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="219e0-136">Relationships</span></span>
<span data-ttu-id="219e0-137">Keine</span><span class="sxs-lookup"><span data-stu-id="219e0-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="219e0-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="219e0-138">JSON representation</span></span>

<span data-ttu-id="219e0-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="219e0-139">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/profilephoto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
