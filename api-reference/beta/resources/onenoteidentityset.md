---
title: Ressourcentyp oneNoteIdentitySet
description: '**Unterstützung in Kürze verfügbar**'
localization_priority: Normal
ms.openlocfilehash: d2969d073503a9fd586641abeb3d82f719db8545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874088"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="1cc00-103">Ressourcentyp oneNoteIdentitySet</span><span class="sxs-lookup"><span data-stu-id="1cc00-103">oneNoteIdentitySet resource type</span></span>

> <span data-ttu-id="1cc00-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1cc00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cc00-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1cc00-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cc00-106">**Unterstützung in Kürze verfügbar**</span><span class="sxs-lookup"><span data-stu-id="1cc00-106">**Support coming soon**</span></span>

<span data-ttu-id="1cc00-107">Der OneNoteIdentitySet-Typ ist eine verschlüsselte Auflistung von [OneNoteIdentity](onenoteidentity.md) -Objekten.</span><span class="sxs-lookup"><span data-stu-id="1cc00-107">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="1cc00-108">Es wird verwendet, um einen Satz von Identitäten zugeordnet sind verschiedene Ereignisse für einen _Notizbuch_, einem _Bereich_ oder einer _Seite_, z. B. _von erstellt_ oder _zuletzt geändert von_darstellen.</span><span class="sxs-lookup"><span data-stu-id="1cc00-108">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="1cc00-109">Aktuell enthält einen einzelnen Schlüssel, _**Benutzer**_.</span><span class="sxs-lookup"><span data-stu-id="1cc00-109">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="1cc00-110">In Zukunft können die Schlüssel wie das Gerät oder einer Anwendung das Element hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="1cc00-110">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="1cc00-111">In Zukunft werden sollen dieses Typs mit [IdentitySet](identityset.md) zusammengeführt</span><span class="sxs-lookup"><span data-stu-id="1cc00-111">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cc00-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1cc00-112">JSON representation</span></span>

<span data-ttu-id="1cc00-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1cc00-113">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="1cc00-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1cc00-114">Properties</span></span>
| <span data-ttu-id="1cc00-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1cc00-115">Property</span></span>     | <span data-ttu-id="1cc00-116">Typ</span><span class="sxs-lookup"><span data-stu-id="1cc00-116">Type</span></span>   |<span data-ttu-id="1cc00-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1cc00-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cc00-118">user</span><span class="sxs-lookup"><span data-stu-id="1cc00-118">user</span></span>|[<span data-ttu-id="1cc00-119">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="1cc00-119">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="1cc00-120">Eine OneNoteIdentity-Ressource, die einen Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="1cc00-120">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
