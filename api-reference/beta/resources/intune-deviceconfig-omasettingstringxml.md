---
title: omaSettingStringXml-Ressourcentyp
description: Zeichenfolgen-XML-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 976c95ed9ffa6674ddc185bb1723c7d7f9d054f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894019"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="d2997-103">omaSettingStringXml-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d2997-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="d2997-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d2997-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2997-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d2997-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2997-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d2997-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2997-107">Zeichenfolgen-XML-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="d2997-107">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="d2997-108">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d2997-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2997-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d2997-109">Properties</span></span>
|<span data-ttu-id="d2997-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2997-110">Property</span></span>|<span data-ttu-id="d2997-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d2997-111">Type</span></span>|<span data-ttu-id="d2997-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2997-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2997-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d2997-113">displayName</span></span>|<span data-ttu-id="d2997-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2997-114">String</span></span>|<span data-ttu-id="d2997-115">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="d2997-115">Display Name.</span></span> <span data-ttu-id="d2997-116">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d2997-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d2997-117">description</span><span class="sxs-lookup"><span data-stu-id="d2997-117">description</span></span>|<span data-ttu-id="d2997-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2997-118">String</span></span>|<span data-ttu-id="d2997-119">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="d2997-119">Description.</span></span> <span data-ttu-id="d2997-120">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d2997-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d2997-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="d2997-121">omaUri</span></span>|<span data-ttu-id="d2997-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2997-122">String</span></span>|<span data-ttu-id="d2997-123">OMA</span><span class="sxs-lookup"><span data-stu-id="d2997-123">OMA.</span></span> <span data-ttu-id="d2997-124">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d2997-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d2997-125">fileName</span><span class="sxs-lookup"><span data-stu-id="d2997-125">fileName</span></span>|<span data-ttu-id="d2997-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2997-126">String</span></span>|<span data-ttu-id="d2997-127">Die dem Dateinamen zugeordnete Werteigenschaft (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="d2997-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="d2997-128">value</span><span class="sxs-lookup"><span data-stu-id="d2997-128">value</span></span>|<span data-ttu-id="d2997-129">Binär</span><span class="sxs-lookup"><span data-stu-id="d2997-129">Binary</span></span>|<span data-ttu-id="d2997-130">Wert</span><span class="sxs-lookup"><span data-stu-id="d2997-130">Value.</span></span> <span data-ttu-id="d2997-131">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="d2997-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2997-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d2997-132">Relationships</span></span>
<span data-ttu-id="d2997-133">Keine</span><span class="sxs-lookup"><span data-stu-id="d2997-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2997-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d2997-134">JSON Representation</span></span>
<span data-ttu-id="d2997-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d2997-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```





