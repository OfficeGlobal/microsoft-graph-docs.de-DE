---
title: Ressourcentyp TeamsTabConfiguration (Open Type)
description: Die Einstellungen, die den Inhalt einer Registerkarte bestimmen.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9873d9e03fec5d7751270b963015aed9eeb0ab48
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953637"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="63433-103">Ressourcentyp TeamsTabConfiguration (Open Type)</span><span class="sxs-lookup"><span data-stu-id="63433-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="63433-104">Die Einstellungen, die den Inhalt einer [Registerkarte](teamstab.md)bestimmen. Wenn eine Registerkarte interaktiv konfiguriert ist, wird diese Informationen von der Registerkarte Anbieter-Anwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63433-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="63433-105">Abgesehen von den Eigenschaften geben Anwendungsbeispiele Anbieter Registerkarte zusätzliche benutzerdefinierte Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="63433-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="63433-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="63433-106">Properties</span></span>

|<span data-ttu-id="63433-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="63433-107">Property</span></span>|<span data-ttu-id="63433-108">Typ</span><span class="sxs-lookup"><span data-stu-id="63433-108">Type</span></span>|<span data-ttu-id="63433-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63433-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="63433-110">entityId</span><span class="sxs-lookup"><span data-stu-id="63433-110">entityId</span></span>   |   <span data-ttu-id="63433-111">string</span><span class="sxs-lookup"><span data-stu-id="63433-111">string</span></span> |  <span data-ttu-id="63433-112">Der Bezeichner für die Entität, die von der Registerkarte Anbieter gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="63433-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="63433-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="63433-113">contentUrl</span></span> |   <span data-ttu-id="63433-114">string</span><span class="sxs-lookup"><span data-stu-id="63433-114">string</span></span> |  <span data-ttu-id="63433-115">URL für das rendering von Inhalt in Teams Registerkarten verwendet.</span><span class="sxs-lookup"><span data-stu-id="63433-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="63433-116">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63433-116">Required.</span></span>    |
|  <span data-ttu-id="63433-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="63433-117">removeUrl</span></span>  |   <span data-ttu-id="63433-118">string</span><span class="sxs-lookup"><span data-stu-id="63433-118">string</span></span> |  <span data-ttu-id="63433-119">URL von Teams Client aufgerufen, wenn eine Registerkarte mithilfe des Teams Clients entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="63433-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="63433-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="63433-120">websiteUrl</span></span> |   <span data-ttu-id="63433-121">string</span><span class="sxs-lookup"><span data-stu-id="63433-121">string</span></span> |  <span data-ttu-id="63433-122">URL für die Anzeige der Registerkarte Inhalt außerhalb von Teams.</span><span class="sxs-lookup"><span data-stu-id="63433-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="63433-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="63433-123">JSON representation</span></span>

<span data-ttu-id="63433-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="63433-124">The following is a JSON representation of the resource.</span></span>
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
