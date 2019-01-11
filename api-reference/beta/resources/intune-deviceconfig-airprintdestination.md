---
title: Ressourcentyp airPrintDestination
description: Stellt ein AirPrint Ziel.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6d1548737956d35d42fc077afe92de1885a54581
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878589"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="9f5a4-103">Ressourcentyp airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="9f5a4-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="9f5a4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f5a4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f5a4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f5a4-107">Stellt ein AirPrint Ziel.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="9f5a4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9f5a4-108">Properties</span></span>
|<span data-ttu-id="9f5a4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f5a4-109">Property</span></span>|<span data-ttu-id="9f5a4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9f5a4-110">Type</span></span>|<span data-ttu-id="9f5a4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f5a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f5a4-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="9f5a4-112">ipAddress</span></span>|<span data-ttu-id="9f5a4-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9f5a4-113">String</span></span>|<span data-ttu-id="9f5a4-114">Die IP-Adresse des Ziels AirPrint.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="9f5a4-115">Http://</span><span class="sxs-lookup"><span data-stu-id="9f5a4-115">resourcePath</span></span>|<span data-ttu-id="9f5a4-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9f5a4-116">String</span></span>|<span data-ttu-id="9f5a4-117">Der Pfad der Ressource mit dem Drucker verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="9f5a4-118">Dies entspricht dem Rp-Parameter, der die _ipps.tcp Bonjour Datensatz.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="9f5a4-119">Beispiel: Drucker/Canon_MG5300_series, Drucker/Xerox_Phaser_7600, Ipp/Epson_IPP_Printer drucken.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="9f5a4-120">port</span><span class="sxs-lookup"><span data-stu-id="9f5a4-120">port</span></span>|<span data-ttu-id="9f5a4-121">Int32</span><span class="sxs-lookup"><span data-stu-id="9f5a4-121">Int32</span></span>|<span data-ttu-id="9f5a4-122">Der Überwachungsport des Ziels AirPrint.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="9f5a4-123">Wenn dieser Schlüssel nicht angegeben ist, wird AirPrint den Standardport verwenden.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="9f5a4-124">In iOS 11.0 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="9f5a4-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="9f5a4-125">forceTls</span></span>|<span data-ttu-id="9f5a4-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9f5a4-126">Boolean</span></span>|<span data-ttu-id="9f5a4-127">Wenn true AirPrint Verbindungen von Transport Layer Security (TLS) gesichert werden.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="9f5a4-128">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-128">Default is false.</span></span> <span data-ttu-id="9f5a4-129">In iOS 11.0 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f5a4-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9f5a4-130">Relationships</span></span>
<span data-ttu-id="9f5a4-131">Keine</span><span class="sxs-lookup"><span data-stu-id="9f5a4-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f5a4-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9f5a4-132">JSON Representation</span></span>
<span data-ttu-id="9f5a4-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9f5a4-133">Here is a JSON representation of the resource.</span></span>
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





