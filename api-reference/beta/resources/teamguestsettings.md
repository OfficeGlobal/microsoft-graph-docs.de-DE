---
title: Ressourcentyp teamGuestSettings
description: Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.
ms.openlocfilehash: 744e19165121d101a720a86bec0242fc31137768
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061815"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="53621-103">Ressourcentyp teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="53621-103">teamGuestSettings resource type</span></span>

> <span data-ttu-id="53621-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53621-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53621-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53621-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53621-106">Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im [Team](team.md)können.</span><span class="sxs-lookup"><span data-stu-id="53621-106">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="53621-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="53621-107">Properties</span></span>
| <span data-ttu-id="53621-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53621-108">Property</span></span>     | <span data-ttu-id="53621-109">Typ</span><span class="sxs-lookup"><span data-stu-id="53621-109">Type</span></span>   |<span data-ttu-id="53621-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53621-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53621-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="53621-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="53621-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="53621-112">Boolean</span></span>|<span data-ttu-id="53621-113">Wenn Festlegung auf "true" Gäste hinzufügen und Kanäle aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="53621-113">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="53621-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="53621-114">allowDeleteChannels</span></span>|<span data-ttu-id="53621-115">Boolesch</span><span class="sxs-lookup"><span data-stu-id="53621-115">Boolean</span></span>|<span data-ttu-id="53621-116">Bei Festlegung auf "true" Gäste Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="53621-116">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53621-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="53621-117">JSON representation</span></span>

<span data-ttu-id="53621-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="53621-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
