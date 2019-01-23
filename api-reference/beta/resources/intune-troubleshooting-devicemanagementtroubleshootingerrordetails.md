---
title: Ressourcentyp deviceManagementTroubleshootingErrorDetails
description: Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9cdda64170afc739c23f1b258e5f2f1b31158662
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430010"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="e3bd3-103">Ressourcentyp deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e3bd3-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="e3bd3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e3bd3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3bd3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3bd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3bd3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3bd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3bd3-107">Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e3bd3-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="e3bd3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3bd3-108">Properties</span></span>
|<span data-ttu-id="e3bd3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3bd3-109">Property</span></span>|<span data-ttu-id="e3bd3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e3bd3-110">Type</span></span>|<span data-ttu-id="e3bd3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3bd3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3bd3-112">context</span><span class="sxs-lookup"><span data-stu-id="e3bd3-112">context</span></span>|<span data-ttu-id="e3bd3-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3bd3-113">String</span></span>|<span data-ttu-id="e3bd3-114">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e3bd3-114">Not yet documented</span></span>|
|<span data-ttu-id="e3bd3-115">failure</span><span class="sxs-lookup"><span data-stu-id="e3bd3-115">failure</span></span>|<span data-ttu-id="e3bd3-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3bd3-116">String</span></span>|<span data-ttu-id="e3bd3-117">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e3bd3-117">Not yet documented</span></span>|
|<span data-ttu-id="e3bd3-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="e3bd3-118">failureDetails</span></span>|<span data-ttu-id="e3bd3-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3bd3-119">String</span></span>|<span data-ttu-id="e3bd3-120">Die detaillierte Beschreibung der Fehlerursache.</span><span class="sxs-lookup"><span data-stu-id="e3bd3-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="e3bd3-121">Wartung</span><span class="sxs-lookup"><span data-stu-id="e3bd3-121">remediation</span></span>|<span data-ttu-id="e3bd3-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3bd3-122">String</span></span>|<span data-ttu-id="e3bd3-123">Die detaillierte Beschreibung der Vorgehensweise zur Behebung dieses Problems.</span><span class="sxs-lookup"><span data-stu-id="e3bd3-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="e3bd3-124">resources</span><span class="sxs-lookup"><span data-stu-id="e3bd3-124">resources</span></span>|<span data-ttu-id="e3bd3-125">[DeviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e3bd3-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="e3bd3-126">Enthält Links zu hilfreiche Dokumentation zu diesem Fehler.</span><span class="sxs-lookup"><span data-stu-id="e3bd3-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3bd3-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3bd3-127">Relationships</span></span>
<span data-ttu-id="e3bd3-128">Keine</span><span class="sxs-lookup"><span data-stu-id="e3bd3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3bd3-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3bd3-129">JSON Representation</span></span>
<span data-ttu-id="e3bd3-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3bd3-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




