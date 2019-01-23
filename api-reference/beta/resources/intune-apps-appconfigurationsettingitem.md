---
title: appConfigurationSettingItem-Ressourcentyp
description: Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7f5492c9b54c9414db6a8332e218a1d7f0a50b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403763"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="8f300-103">appConfigurationSettingItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8f300-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="8f300-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8f300-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f300-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f300-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f300-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f300-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f300-107">Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.</span><span class="sxs-lookup"><span data-stu-id="8f300-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="8f300-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f300-108">Properties</span></span>
|<span data-ttu-id="8f300-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f300-109">Property</span></span>|<span data-ttu-id="8f300-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8f300-110">Type</span></span>|<span data-ttu-id="8f300-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f300-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f300-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="8f300-112">appConfigKey</span></span>|<span data-ttu-id="8f300-113">String</span><span class="sxs-lookup"><span data-stu-id="8f300-113">String</span></span>|<span data-ttu-id="8f300-114">App-Konfigurationsschlüssel</span><span class="sxs-lookup"><span data-stu-id="8f300-114">app configuration key.</span></span>|
|<span data-ttu-id="8f300-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="8f300-115">appConfigKeyType</span></span>|[<span data-ttu-id="8f300-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="8f300-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="8f300-117">Typs des App-Konfigurationsschlüssels.</span><span class="sxs-lookup"><span data-stu-id="8f300-117">app configuration key type.</span></span> <span data-ttu-id="8f300-118">Mögliche Werte: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="8f300-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="8f300-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="8f300-119">appConfigKeyValue</span></span>|<span data-ttu-id="8f300-120">String</span><span class="sxs-lookup"><span data-stu-id="8f300-120">String</span></span>|<span data-ttu-id="8f300-121">Wert des App-Konfigurationsschlüssels</span><span class="sxs-lookup"><span data-stu-id="8f300-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f300-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f300-122">Relationships</span></span>
<span data-ttu-id="8f300-123">Keine</span><span class="sxs-lookup"><span data-stu-id="8f300-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f300-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f300-124">JSON Representation</span></span>
<span data-ttu-id="8f300-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f300-125">Here is a JSON representation of the resource.</span></span>
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




