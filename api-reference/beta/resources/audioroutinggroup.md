---
title: Ressourcentyp audioRoutingGroup
description: Die audio Routinggruppe speichert eine private audio Route zwischen Teilnehmer an einer Unterhaltung mit mehreren Teilnehmern. Quelle der Teilnehmer selbst und die Empfänger sind eine Teilmenge der andere Teilnehmer an der Unterhaltung mit mehreren Teilnehmern.
author: VinodRavichandran
ms.openlocfilehash: 0e1db47963576e728a07a6b99ecff09a0f4640d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344471"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="b9c1c-104">Ressourcentyp audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b9c1c-104">audioRoutingGroup resource type</span></span>

> <span data-ttu-id="b9c1c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9c1c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9c1c-107">Die audio Routinggruppe speichert eine private audio Route zwischen Teilnehmer an einer Unterhaltung mit mehreren Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-107">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="b9c1c-108">Quelle der Teilnehmer selbst und die Empfänger sind eine Teilmenge der andere Teilnehmer an der Unterhaltung mit mehreren Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-108">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="b9c1c-109">**Hinweis:** [ConfigureMixer](../api/participant-configuremixer.md) beinhaltet alle Routen jedoch nicht, ist es für den gesamten Anruf zum Festlegen der Lautstärke für Source-Receiver Kombinationen aus.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-109">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="b9c1c-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="b9c1c-110">Methods</span></span>

| <span data-ttu-id="b9c1c-111">Methode</span><span class="sxs-lookup"><span data-stu-id="b9c1c-111">Method</span></span>                                                  | <span data-ttu-id="b9c1c-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b9c1c-112">Return Type</span></span>                               | <span data-ttu-id="b9c1c-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9c1c-113">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="b9c1c-114">Abrufen von audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b9c1c-114">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="b9c1c-115">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b9c1c-115">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="b9c1c-116">Lesen Sie Eigenschaften und Beziehungen des AudioRoutingGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-116">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="b9c1c-117">Update</span><span class="sxs-lookup"><span data-stu-id="b9c1c-117">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="b9c1c-118">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b9c1c-118">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="b9c1c-119">Aktualisieren Sie Ereignisempfänger Liste.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-119">Update receivers list.</span></span>                       |
| [<span data-ttu-id="b9c1c-120">Delete</span><span class="sxs-lookup"><span data-stu-id="b9c1c-120">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="b9c1c-121">Keine</span><span class="sxs-lookup"><span data-stu-id="b9c1c-121">None</span></span>                                      | <span data-ttu-id="b9c1c-122">Löschen der audio Routinggruppe.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-122">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="b9c1c-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b9c1c-123">Properties</span></span>

| <span data-ttu-id="b9c1c-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9c1c-124">Property</span></span>      | <span data-ttu-id="b9c1c-125">Typ</span><span class="sxs-lookup"><span data-stu-id="b9c1c-125">Type</span></span>              | <span data-ttu-id="b9c1c-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9c1c-126">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="b9c1c-127">id</span><span class="sxs-lookup"><span data-stu-id="b9c1c-127">id</span></span>            | <span data-ttu-id="b9c1c-128">String</span><span class="sxs-lookup"><span data-stu-id="b9c1c-128">String</span></span>            | <span data-ttu-id="b9c1c-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-129">Read-only.</span></span> <span data-ttu-id="b9c1c-130">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-130">Server generated.</span></span>                                         |
| <span data-ttu-id="b9c1c-131">Ereignisempfänger</span><span class="sxs-lookup"><span data-stu-id="b9c1c-131">receivers</span></span>     | <span data-ttu-id="b9c1c-132">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b9c1c-132">String Collection</span></span> | <span data-ttu-id="b9c1c-133">Liste der Teilnehmer Ids empfangen.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-133">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="b9c1c-134">routingMode</span><span class="sxs-lookup"><span data-stu-id="b9c1c-134">routingMode</span></span>   | <span data-ttu-id="b9c1c-135">String</span><span class="sxs-lookup"><span data-stu-id="b9c1c-135">String</span></span>            | <span data-ttu-id="b9c1c-136">Routing Group-Modus.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-136">Routing group mode.</span></span>  <span data-ttu-id="b9c1c-137">Mögliche Werte sind: `oneToOne` und `multicast`.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-137">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="b9c1c-138">sources</span><span class="sxs-lookup"><span data-stu-id="b9c1c-138">sources</span></span>       | <span data-ttu-id="b9c1c-139">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b9c1c-139">String Collection</span></span> | <span data-ttu-id="b9c1c-140">Liste der Teilnehmer Source-Ids.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-140">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="b9c1c-141">**Hinweis:** Routing Modus bestimmt die Einschränkungen auf die Quellen und Ereignisempfänger.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-141">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="b9c1c-142">Die folgenden Routinggruppen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-142">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="b9c1c-143">`oneToOne`-Quellen und Ereignisempfänger nur an einen Teilnehmer haben.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-143">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="b9c1c-144">`multicast`-Quelle ein Teilnehmer hat, aber es gibt mehrere Empfänger.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-144">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="b9c1c-145">Ereignisempfänger möglicherweise aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-145">Receivers list may be updated.</span></span>

> <span data-ttu-id="b9c1c-146">**Hinweis:** Wenn Sie viele Audio-Routinggruppen (z. B. Bot pro Teilnehmer) erstellen, wird nur die Audiodaten der oberen 4 dominanten Lautsprecher weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-146">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="b9c1c-147">Sie bedeutet, dass selbst bei angepassten audio Routinggruppe ist der Lautsprecher nicht laut genug im Hauptfenster Mixer, er den Robot hören, ist nicht möglich, auch wenn eine private audio Gruppe nur für diese Lautsprecher und den Robot vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-147">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="b9c1c-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b9c1c-148">Relationships</span></span>
<span data-ttu-id="b9c1c-149">Keine</span><span class="sxs-lookup"><span data-stu-id="b9c1c-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9c1c-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b9c1c-150">JSON representation</span></span>

<span data-ttu-id="b9c1c-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b9c1c-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
