---
title: Ressourcentyp airPrintDestination
description: Stellt ein AirPrint Ziel.
author: tfitzmac
ms.openlocfilehash: 046f85c65d382b34e6920f30f6b2718f817371a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361054"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="335b2-103">Ressourcentyp airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="335b2-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="335b2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="335b2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="335b2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="335b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="335b2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="335b2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="335b2-107">Stellt ein AirPrint Ziel.</span><span class="sxs-lookup"><span data-stu-id="335b2-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="335b2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="335b2-108">Properties</span></span>
|<span data-ttu-id="335b2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="335b2-109">Property</span></span>|<span data-ttu-id="335b2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="335b2-110">Type</span></span>|<span data-ttu-id="335b2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="335b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="335b2-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="335b2-112">ipAddress</span></span>|<span data-ttu-id="335b2-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="335b2-113">String</span></span>|<span data-ttu-id="335b2-114">Die IP-Adresse des Ziels AirPrint.</span><span class="sxs-lookup"><span data-stu-id="335b2-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="335b2-115">Http://</span><span class="sxs-lookup"><span data-stu-id="335b2-115">resourcePath</span></span>|<span data-ttu-id="335b2-116">String</span><span class="sxs-lookup"><span data-stu-id="335b2-116">String</span></span>|<span data-ttu-id="335b2-117">Der Pfad der Ressource mit dem Drucker verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="335b2-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="335b2-118">Dies entspricht dem Rp-Parameter, der die _ipps.tcp Bonjour Datensatz.</span><span class="sxs-lookup"><span data-stu-id="335b2-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="335b2-119">Beispiel: Drucker/Canon_MG5300_series, Drucker/Xerox_Phaser_7600, Ipp/Epson_IPP_Printer drucken.</span><span class="sxs-lookup"><span data-stu-id="335b2-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="335b2-120">port</span><span class="sxs-lookup"><span data-stu-id="335b2-120">port</span></span>|<span data-ttu-id="335b2-121">Int32</span><span class="sxs-lookup"><span data-stu-id="335b2-121">Int32</span></span>|<span data-ttu-id="335b2-122">Der Überwachungsport des Ziels AirPrint.</span><span class="sxs-lookup"><span data-stu-id="335b2-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="335b2-123">Wenn dieser Schlüssel nicht angegeben ist, wird AirPrint den Standardport verwenden.</span><span class="sxs-lookup"><span data-stu-id="335b2-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="335b2-124">In iOS 11.0 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="335b2-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="335b2-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="335b2-125">forceTls</span></span>|<span data-ttu-id="335b2-126">Boolesch</span><span class="sxs-lookup"><span data-stu-id="335b2-126">Boolean</span></span>|<span data-ttu-id="335b2-127">Wenn true AirPrint Verbindungen von Transport Layer Security (TLS) gesichert werden.</span><span class="sxs-lookup"><span data-stu-id="335b2-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="335b2-128">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="335b2-128">Default is false.</span></span> <span data-ttu-id="335b2-129">In iOS 11.0 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="335b2-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="335b2-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="335b2-130">Relationships</span></span>
<span data-ttu-id="335b2-131">Keine</span><span class="sxs-lookup"><span data-stu-id="335b2-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="335b2-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="335b2-132">JSON Representation</span></span>
<span data-ttu-id="335b2-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="335b2-133">Here is a JSON representation of the resource.</span></span>
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





