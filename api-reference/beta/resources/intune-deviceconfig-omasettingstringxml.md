---
title: omaSettingStringXml-Ressourcentyp
description: Zeichenfolgen-XML-Definition der OMA-Einstellungen
author: tfitzmac
ms.openlocfilehash: 5582ca84a9d6c918ce7b8dea5a21f616804da4ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323786"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="f9221-103">omaSettingStringXml-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f9221-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="f9221-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9221-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9221-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9221-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9221-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f9221-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9221-107">Zeichenfolgen-XML-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="f9221-107">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="f9221-108">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f9221-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f9221-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9221-109">Properties</span></span>
|<span data-ttu-id="f9221-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9221-110">Property</span></span>|<span data-ttu-id="f9221-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f9221-111">Type</span></span>|<span data-ttu-id="f9221-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9221-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9221-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f9221-113">displayName</span></span>|<span data-ttu-id="f9221-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9221-114">String</span></span>|<span data-ttu-id="f9221-115">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="f9221-115">Display Name.</span></span> <span data-ttu-id="f9221-116">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f9221-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f9221-117">description</span><span class="sxs-lookup"><span data-stu-id="f9221-117">description</span></span>|<span data-ttu-id="f9221-118">String</span><span class="sxs-lookup"><span data-stu-id="f9221-118">String</span></span>|<span data-ttu-id="f9221-119">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="f9221-119">Description.</span></span> <span data-ttu-id="f9221-120">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f9221-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f9221-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="f9221-121">omaUri</span></span>|<span data-ttu-id="f9221-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9221-122">String</span></span>|<span data-ttu-id="f9221-123">OMA</span><span class="sxs-lookup"><span data-stu-id="f9221-123">OMA.</span></span> <span data-ttu-id="f9221-124">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f9221-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f9221-125">fileName</span><span class="sxs-lookup"><span data-stu-id="f9221-125">fileName</span></span>|<span data-ttu-id="f9221-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9221-126">String</span></span>|<span data-ttu-id="f9221-127">Die dem Dateinamen zugeordnete Werteigenschaft (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="f9221-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="f9221-128">value</span><span class="sxs-lookup"><span data-stu-id="f9221-128">value</span></span>|<span data-ttu-id="f9221-129">Binär</span><span class="sxs-lookup"><span data-stu-id="f9221-129">Binary</span></span>|<span data-ttu-id="f9221-130">Wert</span><span class="sxs-lookup"><span data-stu-id="f9221-130">Value.</span></span> <span data-ttu-id="f9221-131">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="f9221-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9221-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f9221-132">Relationships</span></span>
<span data-ttu-id="f9221-133">Keine</span><span class="sxs-lookup"><span data-stu-id="f9221-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9221-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9221-134">JSON Representation</span></span>
<span data-ttu-id="f9221-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9221-135">Here is a JSON representation of the resource.</span></span>
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





