---
title: Ressourcentyp osVersionCount
description: Anzahl der Geräte mit Malware für jede Version des Betriebssystems
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbe0d8ac149ad84ba4cd1286fb0f2303cdfb52a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410462"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="1d81d-103">Ressourcentyp osVersionCount</span><span class="sxs-lookup"><span data-stu-id="1d81d-103">osVersionCount resource type</span></span>

> <span data-ttu-id="1d81d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1d81d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d81d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d81d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d81d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1d81d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d81d-107">Anzahl der Geräte mit Malware für jede Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="1d81d-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="1d81d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d81d-108">Properties</span></span>
|<span data-ttu-id="1d81d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d81d-109">Property</span></span>|<span data-ttu-id="1d81d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1d81d-110">Type</span></span>|<span data-ttu-id="1d81d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d81d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d81d-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="1d81d-112">osVersion</span></span>|<span data-ttu-id="1d81d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1d81d-113">String</span></span>|<span data-ttu-id="1d81d-114">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="1d81d-114">OS version</span></span>|
|<span data-ttu-id="1d81d-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1d81d-115">deviceCount</span></span>|<span data-ttu-id="1d81d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1d81d-116">Int32</span></span>|<span data-ttu-id="1d81d-117">Anzahl der Geräte mit Malware für die Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="1d81d-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="1d81d-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1d81d-118">lastUpdateDateTime</span></span>|<span data-ttu-id="1d81d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d81d-119">DateTimeOffset</span></span>|<span data-ttu-id="1d81d-120">Der Zeitstempel der letzten Aktualisierung für die Anzahl der Geräte in UTC</span><span class="sxs-lookup"><span data-stu-id="1d81d-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d81d-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1d81d-121">Relationships</span></span>
<span data-ttu-id="1d81d-122">Keine</span><span class="sxs-lookup"><span data-stu-id="1d81d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d81d-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d81d-123">JSON Representation</span></span>
<span data-ttu-id="1d81d-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1d81d-124">Here is a JSON representation of the resource.</span></span>
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




