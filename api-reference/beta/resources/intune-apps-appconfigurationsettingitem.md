---
title: appConfigurationSettingItem-Ressourcentyp
description: Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddd574ea19057fe31dbca5f258f8153071cd440c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927128"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="1326c-103">appConfigurationSettingItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1326c-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="1326c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1326c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1326c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1326c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1326c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1326c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1326c-107">Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.</span><span class="sxs-lookup"><span data-stu-id="1326c-107">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="1326c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1326c-108">Properties</span></span>
|<span data-ttu-id="1326c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1326c-109">Property</span></span>|<span data-ttu-id="1326c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1326c-110">Type</span></span>|<span data-ttu-id="1326c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1326c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1326c-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="1326c-112">appConfigKey</span></span>|<span data-ttu-id="1326c-113">String</span><span class="sxs-lookup"><span data-stu-id="1326c-113">String</span></span>|<span data-ttu-id="1326c-114">App-Konfigurationsschlüssel</span><span class="sxs-lookup"><span data-stu-id="1326c-114">app configuration key.</span></span>|
|<span data-ttu-id="1326c-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="1326c-115">appConfigKeyType</span></span>|[<span data-ttu-id="1326c-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="1326c-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="1326c-117">Typs des App-Konfigurationsschlüssels.</span><span class="sxs-lookup"><span data-stu-id="1326c-117">app configuration key type.</span></span> <span data-ttu-id="1326c-118">Mögliche Werte: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="1326c-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="1326c-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="1326c-119">appConfigKeyValue</span></span>|<span data-ttu-id="1326c-120">String</span><span class="sxs-lookup"><span data-stu-id="1326c-120">String</span></span>|<span data-ttu-id="1326c-121">Wert des App-Konfigurationsschlüssels</span><span class="sxs-lookup"><span data-stu-id="1326c-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1326c-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1326c-122">Relationships</span></span>
<span data-ttu-id="1326c-123">Keine</span><span class="sxs-lookup"><span data-stu-id="1326c-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1326c-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1326c-124">JSON Representation</span></span>
<span data-ttu-id="1326c-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1326c-125">Here is a JSON representation of the resource.</span></span>
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





