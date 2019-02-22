---
title: osVersionCount-Ressourcentyp
description: Anzahl der Geräte mit Schadsoftware für jede Betriebssystemversion
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12ee68855f45ed6827f84a64084118c24081d266
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142749"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="a3459-103">osVersionCount-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a3459-103">osVersionCount resource type</span></span>

> <span data-ttu-id="a3459-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3459-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3459-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a3459-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3459-106">Anzahl der Geräte mit Schadsoftware für jede Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="a3459-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="a3459-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a3459-107">Properties</span></span>
|<span data-ttu-id="a3459-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3459-108">Property</span></span>|<span data-ttu-id="a3459-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a3459-109">Type</span></span>|<span data-ttu-id="a3459-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3459-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3459-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="a3459-111">osVersion</span></span>|<span data-ttu-id="a3459-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3459-112">String</span></span>|<span data-ttu-id="a3459-113">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="a3459-113">OS version</span></span>|
|<span data-ttu-id="a3459-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a3459-114">deviceCount</span></span>|<span data-ttu-id="a3459-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a3459-115">Int32</span></span>|<span data-ttu-id="a3459-116">Anzahl der Geräte mit Schadsoftware für die Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="a3459-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="a3459-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a3459-117">lastUpdateDateTime</span></span>|<span data-ttu-id="a3459-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3459-118">DateTimeOffset</span></span>|<span data-ttu-id="a3459-119">Der Zeitstempel der letzten Aktualisierung für die Geräteanzahl in UTC</span><span class="sxs-lookup"><span data-stu-id="a3459-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3459-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a3459-120">Relationships</span></span>
<span data-ttu-id="a3459-121">Keine</span><span class="sxs-lookup"><span data-stu-id="a3459-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3459-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a3459-122">JSON Representation</span></span>
<span data-ttu-id="a3459-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a3459-123">Here is a JSON representation of the resource.</span></span>
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




