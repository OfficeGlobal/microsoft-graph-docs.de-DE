---
title: Ressourcentyp audioRoutingGroup
description: Die audio Routinggruppe speichert eine private audio Route zwischen Teilnehmer an einer Unterhaltung mit mehreren Teilnehmern. Quelle der Teilnehmer selbst und die Empfänger sind eine Teilmenge der andere Teilnehmer an der Unterhaltung mit mehreren Teilnehmern.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fb1303e2a6f9e269faf5767093d418cdd0980463
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573018"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="ed9db-104">Ressourcentyp audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="ed9db-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed9db-105">Die audio Routinggruppe speichert eine private audio Route zwischen Teilnehmer an einer Unterhaltung mit mehreren Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="ed9db-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="ed9db-106">Quelle der Teilnehmer selbst und die Empfänger sind eine Teilmenge der andere Teilnehmer an der Unterhaltung mit mehreren Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="ed9db-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="ed9db-107">**Hinweis:** [ConfigureMixer](../api/participant-configuremixer.md) beinhaltet alle Routen jedoch nicht, ist es für den gesamten Anruf zum Festlegen der Lautstärke für Source-Receiver Kombinationen aus.</span><span class="sxs-lookup"><span data-stu-id="ed9db-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="ed9db-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="ed9db-108">Methods</span></span>

| <span data-ttu-id="ed9db-109">Methode</span><span class="sxs-lookup"><span data-stu-id="ed9db-109">Method</span></span>                                                  | <span data-ttu-id="ed9db-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ed9db-110">Return Type</span></span>                               | <span data-ttu-id="ed9db-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed9db-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="ed9db-112">Abrufen von audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="ed9db-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="ed9db-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="ed9db-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="ed9db-114">Lesen Sie Eigenschaften und Beziehungen des AudioRoutingGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ed9db-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="ed9db-115">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ed9db-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="ed9db-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="ed9db-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="ed9db-117">Aktualisieren Sie Ereignisempfänger Liste.</span><span class="sxs-lookup"><span data-stu-id="ed9db-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="ed9db-118">Löschen</span><span class="sxs-lookup"><span data-stu-id="ed9db-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="ed9db-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ed9db-119">None</span></span>                                      | <span data-ttu-id="ed9db-120">Löschen der audio Routinggruppe.</span><span class="sxs-lookup"><span data-stu-id="ed9db-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="ed9db-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed9db-121">Properties</span></span>

| <span data-ttu-id="ed9db-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed9db-122">Property</span></span>      | <span data-ttu-id="ed9db-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ed9db-123">Type</span></span>              | <span data-ttu-id="ed9db-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed9db-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="ed9db-125">id</span><span class="sxs-lookup"><span data-stu-id="ed9db-125">id</span></span>            | <span data-ttu-id="ed9db-126">String</span><span class="sxs-lookup"><span data-stu-id="ed9db-126">String</span></span>            | <span data-ttu-id="ed9db-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed9db-127">Read-only.</span></span> <span data-ttu-id="ed9db-128">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="ed9db-128">Server generated.</span></span>                                         |
| <span data-ttu-id="ed9db-129">Ereignisempfänger</span><span class="sxs-lookup"><span data-stu-id="ed9db-129">receivers</span></span>     | <span data-ttu-id="ed9db-130">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ed9db-130">String Collection</span></span> | <span data-ttu-id="ed9db-131">Liste der Teilnehmer Ids empfangen.</span><span class="sxs-lookup"><span data-stu-id="ed9db-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="ed9db-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="ed9db-132">routingMode</span></span>   | <span data-ttu-id="ed9db-133">String</span><span class="sxs-lookup"><span data-stu-id="ed9db-133">String</span></span>            | <span data-ttu-id="ed9db-134">Routing Group-Modus.</span><span class="sxs-lookup"><span data-stu-id="ed9db-134">Routing group mode.</span></span>  <span data-ttu-id="ed9db-135">Mögliche Werte sind: `oneToOne` und `multicast`.</span><span class="sxs-lookup"><span data-stu-id="ed9db-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="ed9db-136">sources</span><span class="sxs-lookup"><span data-stu-id="ed9db-136">sources</span></span>       | <span data-ttu-id="ed9db-137">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ed9db-137">String Collection</span></span> | <span data-ttu-id="ed9db-138">Liste der Teilnehmer Source-Ids.</span><span class="sxs-lookup"><span data-stu-id="ed9db-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="ed9db-139">**Hinweis:** Routing Modus bestimmt die Einschränkungen auf die Quellen und Ereignisempfänger.</span><span class="sxs-lookup"><span data-stu-id="ed9db-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="ed9db-140">Die folgenden Routinggruppen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed9db-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="ed9db-141">`oneToOne`-Quellen und Ereignisempfänger nur an einen Teilnehmer haben.</span><span class="sxs-lookup"><span data-stu-id="ed9db-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="ed9db-142">`multicast`-Quelle ein Teilnehmer hat, aber es gibt mehrere Empfänger.</span><span class="sxs-lookup"><span data-stu-id="ed9db-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="ed9db-143">Ereignisempfänger möglicherweise aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="ed9db-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="ed9db-144">**Hinweis:** Wenn Sie viele Audio-Routinggruppen (z. B. Bot pro Teilnehmer) erstellen, wird nur die Audiodaten der oberen 4 dominanten Lautsprecher weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="ed9db-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="ed9db-145">Sie bedeutet, dass selbst bei angepassten audio Routinggruppe ist der Lautsprecher nicht laut genug im Hauptfenster Mixer, er den Robot hören, ist nicht möglich, auch wenn eine private audio Gruppe nur für diese Lautsprecher und den Robot vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="ed9db-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="ed9db-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ed9db-146">Relationships</span></span>
<span data-ttu-id="ed9db-147">Keine</span><span class="sxs-lookup"><span data-stu-id="ed9db-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed9db-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ed9db-148">JSON representation</span></span>

<span data-ttu-id="ed9db-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ed9db-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "Guid" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "Guid" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
