---
title: appConfigurationSettingItem-Ressourcentyp
description: Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.
author: tfitzmac
ms.openlocfilehash: b75579e56602ad5359bc32d52312931342b42a6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353578"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="e4026-103">appConfigurationSettingItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e4026-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="e4026-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4026-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4026-105">Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.</span><span class="sxs-lookup"><span data-stu-id="e4026-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="e4026-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e4026-106">Properties</span></span>
|<span data-ttu-id="e4026-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4026-107">Property</span></span>|<span data-ttu-id="e4026-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e4026-108">Type</span></span>|<span data-ttu-id="e4026-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4026-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4026-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="e4026-110">appConfigKey</span></span>|<span data-ttu-id="e4026-111">String</span><span class="sxs-lookup"><span data-stu-id="e4026-111">String</span></span>|<span data-ttu-id="e4026-112">App-Konfigurationsschlüssel</span><span class="sxs-lookup"><span data-stu-id="e4026-112">app configuration key.</span></span>|
|<span data-ttu-id="e4026-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e4026-113">appConfigKeyType</span></span>|[<span data-ttu-id="e4026-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e4026-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="e4026-115">Typs des App-Konfigurationsschlüssels.</span><span class="sxs-lookup"><span data-stu-id="e4026-115">app configuration key type.</span></span> <span data-ttu-id="e4026-116">Mögliche Werte: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="e4026-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="e4026-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="e4026-117">appConfigKeyValue</span></span>|<span data-ttu-id="e4026-118">String</span><span class="sxs-lookup"><span data-stu-id="e4026-118">String</span></span>|<span data-ttu-id="e4026-119">Wert des App-Konfigurationsschlüssels</span><span class="sxs-lookup"><span data-stu-id="e4026-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4026-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e4026-120">Relationships</span></span>
<span data-ttu-id="e4026-121">Keine</span><span class="sxs-lookup"><span data-stu-id="e4026-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4026-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e4026-122">JSON Representation</span></span>
<span data-ttu-id="e4026-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e4026-123">Here is a JSON representation of the resource.</span></span>
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



