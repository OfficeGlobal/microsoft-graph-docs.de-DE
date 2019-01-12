---
title: Ressourcentyp airPrintDestination
description: Stellt ein AirPrint Ziel.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ede4f580557e75d206e0b429069acb13f81bcc5f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962513"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="a35fb-103">Ressourcentyp airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="a35fb-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="a35fb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a35fb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a35fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a35fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a35fb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a35fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a35fb-107">Stellt ein AirPrint Ziel.</span><span class="sxs-lookup"><span data-stu-id="a35fb-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="a35fb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a35fb-108">Properties</span></span>
|<span data-ttu-id="a35fb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a35fb-109">Property</span></span>|<span data-ttu-id="a35fb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a35fb-110">Type</span></span>|<span data-ttu-id="a35fb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a35fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a35fb-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="a35fb-112">ipAddress</span></span>|<span data-ttu-id="a35fb-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a35fb-113">String</span></span>|<span data-ttu-id="a35fb-114">Die IP-Adresse des Ziels AirPrint.</span><span class="sxs-lookup"><span data-stu-id="a35fb-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="a35fb-115">Http://</span><span class="sxs-lookup"><span data-stu-id="a35fb-115">resourcePath</span></span>|<span data-ttu-id="a35fb-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a35fb-116">String</span></span>|<span data-ttu-id="a35fb-117">Der Pfad der Ressource mit dem Drucker verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="a35fb-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="a35fb-118">Dies entspricht dem Rp-Parameter, der die _ipps.tcp Bonjour Datensatz.</span><span class="sxs-lookup"><span data-stu-id="a35fb-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="a35fb-119">Beispiel: Drucker/Canon_MG5300_series, Drucker/Xerox_Phaser_7600, Ipp/Epson_IPP_Printer drucken.</span><span class="sxs-lookup"><span data-stu-id="a35fb-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="a35fb-120">port</span><span class="sxs-lookup"><span data-stu-id="a35fb-120">port</span></span>|<span data-ttu-id="a35fb-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a35fb-121">Int32</span></span>|<span data-ttu-id="a35fb-122">Der Überwachungsport des Ziels AirPrint.</span><span class="sxs-lookup"><span data-stu-id="a35fb-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="a35fb-123">Wenn dieser Schlüssel nicht angegeben ist, wird AirPrint den Standardport verwenden.</span><span class="sxs-lookup"><span data-stu-id="a35fb-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="a35fb-124">In iOS 11.0 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a35fb-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="a35fb-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="a35fb-125">forceTls</span></span>|<span data-ttu-id="a35fb-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a35fb-126">Boolean</span></span>|<span data-ttu-id="a35fb-127">Wenn true AirPrint Verbindungen von Transport Layer Security (TLS) gesichert werden.</span><span class="sxs-lookup"><span data-stu-id="a35fb-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="a35fb-128">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="a35fb-128">Default is false.</span></span> <span data-ttu-id="a35fb-129">In iOS 11.0 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a35fb-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a35fb-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a35fb-130">Relationships</span></span>
<span data-ttu-id="a35fb-131">Keine</span><span class="sxs-lookup"><span data-stu-id="a35fb-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a35fb-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a35fb-132">JSON Representation</span></span>
<span data-ttu-id="a35fb-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a35fb-133">Here is a JSON representation of the resource.</span></span>
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





