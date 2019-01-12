---
title: Ressourcentyp osVersionCount
description: Anzahl der Geräte mit Malware für jede Version des Betriebssystems
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de841e679ede22492d26f2a1587e775179c45761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911840"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="99128-103">Ressourcentyp osVersionCount</span><span class="sxs-lookup"><span data-stu-id="99128-103">osVersionCount resource type</span></span>

> <span data-ttu-id="99128-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99128-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99128-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99128-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99128-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="99128-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99128-107">Anzahl der Geräte mit Malware für jede Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="99128-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="99128-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="99128-108">Properties</span></span>
|<span data-ttu-id="99128-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99128-109">Property</span></span>|<span data-ttu-id="99128-110">Typ</span><span class="sxs-lookup"><span data-stu-id="99128-110">Type</span></span>|<span data-ttu-id="99128-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99128-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99128-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="99128-112">osVersion</span></span>|<span data-ttu-id="99128-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99128-113">String</span></span>|<span data-ttu-id="99128-114">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="99128-114">OS version</span></span>|
|<span data-ttu-id="99128-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="99128-115">deviceCount</span></span>|<span data-ttu-id="99128-116">Int32</span><span class="sxs-lookup"><span data-stu-id="99128-116">Int32</span></span>|<span data-ttu-id="99128-117">Anzahl der Geräte mit Malware für die Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="99128-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="99128-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="99128-118">lastUpdateDateTime</span></span>|<span data-ttu-id="99128-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99128-119">DateTimeOffset</span></span>|<span data-ttu-id="99128-120">Der Zeitstempel der letzten Aktualisierung für die Anzahl der Geräte in UTC</span><span class="sxs-lookup"><span data-stu-id="99128-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="99128-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="99128-121">Relationships</span></span>
<span data-ttu-id="99128-122">Keine</span><span class="sxs-lookup"><span data-stu-id="99128-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99128-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="99128-123">JSON Representation</span></span>
<span data-ttu-id="99128-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="99128-124">Here is a JSON representation of the resource.</span></span>
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





