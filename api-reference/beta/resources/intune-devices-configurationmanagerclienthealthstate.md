---
title: configurationManagerClientHealthState-Ressourcentyp
description: Konfigurations-Manager-Client – Integritätsstatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a2d4083554f40bba138c5f886dfa77ad6c54a1d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159745"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="2d104-103">configurationManagerClientHealthState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2d104-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="2d104-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d104-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d104-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2d104-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d104-106">Konfigurations-Manager-Client – Integritätsstatus</span><span class="sxs-lookup"><span data-stu-id="2d104-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="2d104-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2d104-107">Properties</span></span>
|<span data-ttu-id="2d104-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d104-108">Property</span></span>|<span data-ttu-id="2d104-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2d104-109">Type</span></span>|<span data-ttu-id="2d104-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d104-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d104-111">state</span><span class="sxs-lookup"><span data-stu-id="2d104-111">state</span></span>|[<span data-ttu-id="2d104-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="2d104-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="2d104-113">Aktueller Configuration Manager-Clientstatus.</span><span class="sxs-lookup"><span data-stu-id="2d104-113">Current configuration manager client state.</span></span> <span data-ttu-id="2d104-114">Mögliche Werte sind: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed` und `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="2d104-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="2d104-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="2d104-115">errorCode</span></span>|<span data-ttu-id="2d104-116">Int32</span><span class="sxs-lookup"><span data-stu-id="2d104-116">Int32</span></span>|<span data-ttu-id="2d104-117">Fehlercode für fehlgeschlagenen Status.</span><span class="sxs-lookup"><span data-stu-id="2d104-117">Error code for failed state.</span></span>|
|<span data-ttu-id="2d104-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2d104-118">lastSyncDateTime</span></span>|<span data-ttu-id="2d104-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d104-119">DateTimeOffset</span></span>|<span data-ttu-id="2d104-120">DateTime für die letzte Synchronisierung mit Configuration Manager-Verwaltungspunkt.</span><span class="sxs-lookup"><span data-stu-id="2d104-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d104-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2d104-121">Relationships</span></span>
<span data-ttu-id="2d104-122">Keine</span><span class="sxs-lookup"><span data-stu-id="2d104-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d104-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2d104-123">JSON Representation</span></span>
<span data-ttu-id="2d104-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2d104-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```




