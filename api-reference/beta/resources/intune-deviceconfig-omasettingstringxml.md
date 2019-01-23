---
title: omaSettingStringXml-Ressourcentyp
description: Zeichenfolgen-XML-Definition der OMA-Einstellungen
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c0e47ba7fce929e114282c6aa88605d9f185618
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419436"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="1ab88-103">omaSettingStringXml-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1ab88-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="1ab88-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1ab88-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1ab88-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ab88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ab88-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ab88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ab88-107">Zeichenfolgen-XML-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="1ab88-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="1ab88-108">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ab88-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ab88-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1ab88-109">Properties</span></span>
|<span data-ttu-id="1ab88-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ab88-110">Property</span></span>|<span data-ttu-id="1ab88-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1ab88-111">Type</span></span>|<span data-ttu-id="1ab88-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ab88-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ab88-113">displayName</span><span class="sxs-lookup"><span data-stu-id="1ab88-113">displayName</span></span>|<span data-ttu-id="1ab88-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ab88-114">String</span></span>|<span data-ttu-id="1ab88-115">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="1ab88-115">Display Name.</span></span> <span data-ttu-id="1ab88-116">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ab88-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1ab88-117">description</span><span class="sxs-lookup"><span data-stu-id="1ab88-117">description</span></span>|<span data-ttu-id="1ab88-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ab88-118">String</span></span>|<span data-ttu-id="1ab88-119">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="1ab88-119">Description.</span></span> <span data-ttu-id="1ab88-120">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ab88-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1ab88-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="1ab88-121">omaUri</span></span>|<span data-ttu-id="1ab88-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ab88-122">String</span></span>|<span data-ttu-id="1ab88-123">OMA</span><span class="sxs-lookup"><span data-stu-id="1ab88-123">OMA.</span></span> <span data-ttu-id="1ab88-124">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ab88-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1ab88-125">fileName</span><span class="sxs-lookup"><span data-stu-id="1ab88-125">fileName</span></span>|<span data-ttu-id="1ab88-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ab88-126">String</span></span>|<span data-ttu-id="1ab88-127">Die dem Dateinamen zugeordnete Werteigenschaft (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="1ab88-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="1ab88-128">value</span><span class="sxs-lookup"><span data-stu-id="1ab88-128">value</span></span>|<span data-ttu-id="1ab88-129">Binär</span><span class="sxs-lookup"><span data-stu-id="1ab88-129">Binary</span></span>|<span data-ttu-id="1ab88-130">Wert</span><span class="sxs-lookup"><span data-stu-id="1ab88-130">Value.</span></span> <span data-ttu-id="1ab88-131">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="1ab88-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ab88-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1ab88-132">Relationships</span></span>
<span data-ttu-id="1ab88-133">Keine</span><span class="sxs-lookup"><span data-stu-id="1ab88-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ab88-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1ab88-134">JSON Representation</span></span>
<span data-ttu-id="1ab88-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1ab88-135">Here is a JSON representation of the resource.</span></span>
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




