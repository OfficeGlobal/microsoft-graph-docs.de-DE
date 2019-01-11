---
title: Ressourcentyp osVersionCount
description: Anzahl der Geräte mit Malware für jede Version des Betriebssystems
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 227e802de7226d653d68997268c9bf4eac4aa259
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864148"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="fbfe5-103">Ressourcentyp osVersionCount</span><span class="sxs-lookup"><span data-stu-id="fbfe5-103">osVersionCount resource type</span></span>

> <span data-ttu-id="fbfe5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fbfe5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbfe5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fbfe5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbfe5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fbfe5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbfe5-107">Anzahl der Geräte mit Malware für jede Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="fbfe5-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="fbfe5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fbfe5-108">Properties</span></span>
|<span data-ttu-id="fbfe5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fbfe5-109">Property</span></span>|<span data-ttu-id="fbfe5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fbfe5-110">Type</span></span>|<span data-ttu-id="fbfe5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fbfe5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbfe5-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="fbfe5-112">osVersion</span></span>|<span data-ttu-id="fbfe5-113">String</span><span class="sxs-lookup"><span data-stu-id="fbfe5-113">String</span></span>|<span data-ttu-id="fbfe5-114">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="fbfe5-114">OS version</span></span>|
|<span data-ttu-id="fbfe5-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="fbfe5-115">deviceCount</span></span>|<span data-ttu-id="fbfe5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fbfe5-116">Int32</span></span>|<span data-ttu-id="fbfe5-117">Anzahl der Geräte mit Malware für die Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="fbfe5-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="fbfe5-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="fbfe5-118">lastUpdateDateTime</span></span>|<span data-ttu-id="fbfe5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbfe5-119">DateTimeOffset</span></span>|<span data-ttu-id="fbfe5-120">Der Zeitstempel der letzten Aktualisierung für die Anzahl der Geräte in UTC</span><span class="sxs-lookup"><span data-stu-id="fbfe5-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbfe5-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fbfe5-121">Relationships</span></span>
<span data-ttu-id="fbfe5-122">Keine</span><span class="sxs-lookup"><span data-stu-id="fbfe5-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbfe5-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fbfe5-123">JSON Representation</span></span>
<span data-ttu-id="fbfe5-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fbfe5-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```





