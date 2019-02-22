---
title: appConfigurationSettingItem-Ressourcentyp
description: Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b6b956dcca7ed3540972bae6ff2ba130baaae3f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144492"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="f4343-103">appConfigurationSettingItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f4343-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="f4343-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4343-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4343-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f4343-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4343-106">Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.</span><span class="sxs-lookup"><span data-stu-id="f4343-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="f4343-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f4343-107">Properties</span></span>
|<span data-ttu-id="f4343-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4343-108">Property</span></span>|<span data-ttu-id="f4343-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f4343-109">Type</span></span>|<span data-ttu-id="f4343-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4343-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4343-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="f4343-111">appConfigKey</span></span>|<span data-ttu-id="f4343-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4343-112">String</span></span>|<span data-ttu-id="f4343-113">App-Konfigurationsschlüssel</span><span class="sxs-lookup"><span data-stu-id="f4343-113">app configuration key.</span></span>|
|<span data-ttu-id="f4343-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="f4343-114">appConfigKeyType</span></span>|[<span data-ttu-id="f4343-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="f4343-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="f4343-116">Typs des App-Konfigurationsschlüssels.</span><span class="sxs-lookup"><span data-stu-id="f4343-116">app configuration key type.</span></span> <span data-ttu-id="f4343-117">Mögliche Werte: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="f4343-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="f4343-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="f4343-118">appConfigKeyValue</span></span>|<span data-ttu-id="f4343-119">String</span><span class="sxs-lookup"><span data-stu-id="f4343-119">String</span></span>|<span data-ttu-id="f4343-120">Wert des App-Konfigurationsschlüssels</span><span class="sxs-lookup"><span data-stu-id="f4343-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4343-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f4343-121">Relationships</span></span>
<span data-ttu-id="f4343-122">Keine</span><span class="sxs-lookup"><span data-stu-id="f4343-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4343-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f4343-123">JSON Representation</span></span>
<span data-ttu-id="f4343-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f4343-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```




