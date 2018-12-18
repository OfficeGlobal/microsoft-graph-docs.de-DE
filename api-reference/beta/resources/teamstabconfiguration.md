---
title: Ressourcentyp TeamsTabConfiguration (Open Type)
description: Die Einstellungen, die den Inhalt einer Registerkarte bestimmen.
author: nkramer
ms.openlocfilehash: 9abb4e9089da760825b29c4001b68881ab74d815
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301183"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="b8464-103">Ressourcentyp TeamsTabConfiguration (Open Type)</span><span class="sxs-lookup"><span data-stu-id="b8464-103">teamsTabConfiguration resource type (Open Type)</span></span>

> <span data-ttu-id="b8464-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8464-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8464-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8464-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8464-106">Die Einstellungen, die den Inhalt einer [Registerkarte](teamstab.md)bestimmen. Wenn eine Registerkarte interaktiv konfiguriert ist, wird diese Informationen von der Registerkarte Anbieter-Anwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b8464-106">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="b8464-107">Abgesehen von den Eigenschaften geben Anwendungsbeispiele Anbieter Registerkarte zusätzliche benutzerdefinierte Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="b8464-107">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="b8464-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8464-108">Properties</span></span>

|<span data-ttu-id="b8464-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8464-109">Property</span></span>|<span data-ttu-id="b8464-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b8464-110">Type</span></span>|<span data-ttu-id="b8464-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8464-111">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="b8464-112">entityId</span><span class="sxs-lookup"><span data-stu-id="b8464-112">entityId</span></span>   |   <span data-ttu-id="b8464-113">string</span><span class="sxs-lookup"><span data-stu-id="b8464-113">string</span></span> |  <span data-ttu-id="b8464-114">Der Bezeichner für die Entität, die von der Registerkarte Anbieter gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="b8464-114">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="b8464-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="b8464-115">contentUrl</span></span> |   <span data-ttu-id="b8464-116">string</span><span class="sxs-lookup"><span data-stu-id="b8464-116">string</span></span> |  <span data-ttu-id="b8464-117">URL für das rendering von Inhalt in Teams Registerkarten verwendet.</span><span class="sxs-lookup"><span data-stu-id="b8464-117">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="b8464-118">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8464-118">Required.</span></span>    |
|  <span data-ttu-id="b8464-119">removeUrl</span><span class="sxs-lookup"><span data-stu-id="b8464-119">removeUrl</span></span>  |   <span data-ttu-id="b8464-120">string</span><span class="sxs-lookup"><span data-stu-id="b8464-120">string</span></span> |  <span data-ttu-id="b8464-121">URL von Teams Client aufgerufen, wenn eine Registerkarte mithilfe des Teams Clients entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="b8464-121">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="b8464-122">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="b8464-122">websiteUrl</span></span> |   <span data-ttu-id="b8464-123">string</span><span class="sxs-lookup"><span data-stu-id="b8464-123">string</span></span> |  <span data-ttu-id="b8464-124">URL für die Anzeige der Registerkarte Inhalt außerhalb von Teams.</span><span class="sxs-lookup"><span data-stu-id="b8464-124">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="b8464-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8464-125">JSON representation</span></span>

<span data-ttu-id="b8464-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8464-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
