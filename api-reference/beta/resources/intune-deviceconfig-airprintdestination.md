---
title: airPrintDestination-Ressourcentyp
description: Stellt ein Druckziel dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09301bd791b5fd8b3fa430b50f7cdf58de43944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167333"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="d2555-103">airPrintDestination-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d2555-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="d2555-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d2555-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2555-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d2555-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2555-106">Stellt ein Druckziel dar.</span><span class="sxs-lookup"><span data-stu-id="d2555-106">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="d2555-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d2555-107">Properties</span></span>
|<span data-ttu-id="d2555-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2555-108">Property</span></span>|<span data-ttu-id="d2555-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d2555-109">Type</span></span>|<span data-ttu-id="d2555-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2555-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2555-111">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d2555-111">ipAddress</span></span>|<span data-ttu-id="d2555-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2555-112">String</span></span>|<span data-ttu-id="d2555-113">Die IP-Adresse des Druckziels.</span><span class="sxs-lookup"><span data-stu-id="d2555-113">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="d2555-114">resourcePath</span><span class="sxs-lookup"><span data-stu-id="d2555-114">resourcePath</span></span>|<span data-ttu-id="d2555-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2555-115">String</span></span>|<span data-ttu-id="d2555-116">Der dem Drucker zugeordnete Ressourcenpfad.</span><span class="sxs-lookup"><span data-stu-id="d2555-116">The Resource Path associated with the printer.</span></span> <span data-ttu-id="d2555-117">Dies entspricht dem RP-Parameter des Bonjour-Eintrags _ipps. TCP.</span><span class="sxs-lookup"><span data-stu-id="d2555-117">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="d2555-118">Beispiel: Printers/Canon_MG5300_series, Printers/Xerox_Phaser_7600, IPP/Print, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="d2555-118">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="d2555-119">port</span><span class="sxs-lookup"><span data-stu-id="d2555-119">port</span></span>|<span data-ttu-id="d2555-120">Int32</span><span class="sxs-lookup"><span data-stu-id="d2555-120">Int32</span></span>|<span data-ttu-id="d2555-121">Der Überwachungs-Port des Druckziels.</span><span class="sxs-lookup"><span data-stu-id="d2555-121">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="d2555-122">Wenn dieser Schlüssel nicht angegeben ist, verwendet der standardmäßige Port.</span><span class="sxs-lookup"><span data-stu-id="d2555-122">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="d2555-123">Verfügbar in iOS 11,0 und höher.</span><span class="sxs-lookup"><span data-stu-id="d2555-123">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="d2555-124">forceTls</span><span class="sxs-lookup"><span data-stu-id="d2555-124">forceTls</span></span>|<span data-ttu-id="d2555-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d2555-125">Boolean</span></span>|<span data-ttu-id="d2555-126">Wenn true-druckverbindungs Verbindungen durch Transport Layer Security (TLS) gesichert werden.</span><span class="sxs-lookup"><span data-stu-id="d2555-126">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="d2555-127">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="d2555-127">Default is false.</span></span> <span data-ttu-id="d2555-128">Verfügbar in iOS 11,0 und höher.</span><span class="sxs-lookup"><span data-stu-id="d2555-128">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2555-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d2555-129">Relationships</span></span>
<span data-ttu-id="d2555-130">Keine</span><span class="sxs-lookup"><span data-stu-id="d2555-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2555-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d2555-131">JSON Representation</span></span>
<span data-ttu-id="d2555-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d2555-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```




