---
title: Ressourcentyp oneNoteIdentitySet
description: '**Unterstützung in Kürze verfügbar**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e149d5548ce3585bbcda1f0a199fa97d7543af77
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516714"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="12df8-103">Ressourcentyp oneNoteIdentitySet</span><span class="sxs-lookup"><span data-stu-id="12df8-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12df8-104">**Unterstützung in Kürze verfügbar**</span><span class="sxs-lookup"><span data-stu-id="12df8-104">**Support coming soon**</span></span>

<span data-ttu-id="12df8-105">Der OneNoteIdentitySet-Typ ist eine verschlüsselte Auflistung von [OneNoteIdentity](onenoteidentity.md) -Objekten.</span><span class="sxs-lookup"><span data-stu-id="12df8-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="12df8-106">Es wird verwendet, um einen Satz von Identitäten zugeordnet sind verschiedene Ereignisse für einen _Notizbuch_, einem _Bereich_ oder einer _Seite_, z. B. _von erstellt_ oder _zuletzt geändert von_darstellen.</span><span class="sxs-lookup"><span data-stu-id="12df8-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="12df8-107">Aktuell enthält einen einzelnen Schlüssel, _**Benutzer**_.</span><span class="sxs-lookup"><span data-stu-id="12df8-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="12df8-108">In Zukunft können die Schlüssel wie das Gerät oder einer Anwendung das Element hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="12df8-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="12df8-109">In Zukunft werden sollen dieses Typs mit [IdentitySet](identityset.md) zusammengeführt</span><span class="sxs-lookup"><span data-stu-id="12df8-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="12df8-110">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="12df8-110">JSON representation</span></span>

<span data-ttu-id="12df8-111">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="12df8-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="12df8-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12df8-112">Properties</span></span>
| <span data-ttu-id="12df8-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12df8-113">Property</span></span>     | <span data-ttu-id="12df8-114">Typ</span><span class="sxs-lookup"><span data-stu-id="12df8-114">Type</span></span>   |<span data-ttu-id="12df8-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12df8-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12df8-116">user</span><span class="sxs-lookup"><span data-stu-id="12df8-116">user</span></span>|[<span data-ttu-id="12df8-117">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="12df8-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="12df8-118">Eine OneNoteIdentity-Ressource, die einen Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="12df8-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentityset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
