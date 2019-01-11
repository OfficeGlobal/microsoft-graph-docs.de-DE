---
title: appConfigurationSettingItem-Ressourcentyp
description: Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0590a22178935e9e8a6b4eb0e279b55d4f984222
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842154"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="65caf-103">appConfigurationSettingItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="65caf-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="65caf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65caf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65caf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65caf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65caf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="65caf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65caf-107">Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.</span><span class="sxs-lookup"><span data-stu-id="65caf-107">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="65caf-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="65caf-108">Properties</span></span>
|<span data-ttu-id="65caf-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65caf-109">Property</span></span>|<span data-ttu-id="65caf-110">Typ</span><span class="sxs-lookup"><span data-stu-id="65caf-110">Type</span></span>|<span data-ttu-id="65caf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65caf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65caf-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="65caf-112">appConfigKey</span></span>|<span data-ttu-id="65caf-113">String</span><span class="sxs-lookup"><span data-stu-id="65caf-113">String</span></span>|<span data-ttu-id="65caf-114">App-Konfigurationsschlüssel</span><span class="sxs-lookup"><span data-stu-id="65caf-114">app configuration key.</span></span>|
|<span data-ttu-id="65caf-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="65caf-115">appConfigKeyType</span></span>|[<span data-ttu-id="65caf-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="65caf-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="65caf-117">Typs des App-Konfigurationsschlüssels.</span><span class="sxs-lookup"><span data-stu-id="65caf-117">app configuration key type.</span></span> <span data-ttu-id="65caf-118">Mögliche Werte: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="65caf-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="65caf-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="65caf-119">appConfigKeyValue</span></span>|<span data-ttu-id="65caf-120">String</span><span class="sxs-lookup"><span data-stu-id="65caf-120">String</span></span>|<span data-ttu-id="65caf-121">Wert des App-Konfigurationsschlüssels</span><span class="sxs-lookup"><span data-stu-id="65caf-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65caf-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="65caf-122">Relationships</span></span>
<span data-ttu-id="65caf-123">Keine</span><span class="sxs-lookup"><span data-stu-id="65caf-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65caf-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="65caf-124">JSON Representation</span></span>
<span data-ttu-id="65caf-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="65caf-125">Here is a JSON representation of the resource.</span></span>
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





