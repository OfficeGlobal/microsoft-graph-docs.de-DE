---
title: Ressourcentyp airPrintDestination
description: Stellt ein AirPrint Ziel.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422495"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="c2d8a-103">Ressourcentyp airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="c2d8a-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="c2d8a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2d8a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2d8a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2d8a-107">Stellt ein AirPrint Ziel.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="c2d8a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c2d8a-108">Properties</span></span>
|<span data-ttu-id="c2d8a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c2d8a-109">Property</span></span>|<span data-ttu-id="c2d8a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c2d8a-110">Type</span></span>|<span data-ttu-id="c2d8a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2d8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d8a-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c2d8a-112">ipAddress</span></span>|<span data-ttu-id="c2d8a-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2d8a-113">String</span></span>|<span data-ttu-id="c2d8a-114">Die IP-Adresse des Ziels AirPrint.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="c2d8a-115">Http://</span><span class="sxs-lookup"><span data-stu-id="c2d8a-115">resourcePath</span></span>|<span data-ttu-id="c2d8a-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2d8a-116">String</span></span>|<span data-ttu-id="c2d8a-117">Der Pfad der Ressource mit dem Drucker verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="c2d8a-118">Dies entspricht dem Rp-Parameter, der die _ipps.tcp Bonjour Datensatz.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="c2d8a-119">Beispiel: Drucker/Canon_MG5300_series, Drucker/Xerox_Phaser_7600, Ipp/Epson_IPP_Printer drucken.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="c2d8a-120">port</span><span class="sxs-lookup"><span data-stu-id="c2d8a-120">port</span></span>|<span data-ttu-id="c2d8a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c2d8a-121">Int32</span></span>|<span data-ttu-id="c2d8a-122">Der Überwachungsport des Ziels AirPrint.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="c2d8a-123">Wenn dieser Schlüssel nicht angegeben ist, wird AirPrint den Standardport verwenden.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="c2d8a-124">In iOS 11.0 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="c2d8a-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="c2d8a-125">forceTls</span></span>|<span data-ttu-id="c2d8a-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2d8a-126">Boolean</span></span>|<span data-ttu-id="c2d8a-127">Wenn true AirPrint Verbindungen von Transport Layer Security (TLS) gesichert werden.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="c2d8a-128">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-128">Default is false.</span></span> <span data-ttu-id="c2d8a-129">In iOS 11.0 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2d8a-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c2d8a-130">Relationships</span></span>
<span data-ttu-id="c2d8a-131">Keine</span><span class="sxs-lookup"><span data-stu-id="c2d8a-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2d8a-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c2d8a-132">JSON Representation</span></span>
<span data-ttu-id="c2d8a-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c2d8a-133">Here is a JSON representation of the resource.</span></span>
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




