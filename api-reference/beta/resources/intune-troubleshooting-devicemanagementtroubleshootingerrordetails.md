---
title: deviceManagementTroubleshootingErrorDetails-Ressourcentyp
description: Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08ad43b717a5e08229054bc10aa81a0786f4e344
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142581"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="fa125-103">deviceManagementTroubleshootingErrorDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fa125-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="fa125-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa125-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa125-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fa125-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa125-106">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="fa125-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="fa125-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fa125-107">Properties</span></span>
|<span data-ttu-id="fa125-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa125-108">Property</span></span>|<span data-ttu-id="fa125-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fa125-109">Type</span></span>|<span data-ttu-id="fa125-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa125-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa125-111">context</span><span class="sxs-lookup"><span data-stu-id="fa125-111">context</span></span>|<span data-ttu-id="fa125-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa125-112">String</span></span>|<span data-ttu-id="fa125-113">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fa125-113">Not yet documented</span></span>|
|<span data-ttu-id="fa125-114">failure</span><span class="sxs-lookup"><span data-stu-id="fa125-114">failure</span></span>|<span data-ttu-id="fa125-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa125-115">String</span></span>|<span data-ttu-id="fa125-116">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fa125-116">Not yet documented</span></span>|
|<span data-ttu-id="fa125-117">failureDetails</span><span class="sxs-lookup"><span data-stu-id="fa125-117">failureDetails</span></span>|<span data-ttu-id="fa125-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa125-118">String</span></span>|<span data-ttu-id="fa125-119">Die genaue Beschreibung der Fehler.</span><span class="sxs-lookup"><span data-stu-id="fa125-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="fa125-120">Sanierung</span><span class="sxs-lookup"><span data-stu-id="fa125-120">remediation</span></span>|<span data-ttu-id="fa125-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa125-121">String</span></span>|<span data-ttu-id="fa125-122">Die ausführliche Beschreibung der Problembehebung.</span><span class="sxs-lookup"><span data-stu-id="fa125-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="fa125-123">resources</span><span class="sxs-lookup"><span data-stu-id="fa125-123">resources</span></span>|<span data-ttu-id="fa125-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="fa125-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="fa125-125">Links zu hilfreichen Dokumentationen zu diesem Misserfolg.</span><span class="sxs-lookup"><span data-stu-id="fa125-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa125-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fa125-126">Relationships</span></span>
<span data-ttu-id="fa125-127">Keine</span><span class="sxs-lookup"><span data-stu-id="fa125-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa125-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fa125-128">JSON Representation</span></span>
<span data-ttu-id="fa125-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa125-129">Here is a JSON representation of the resource.</span></span>
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




