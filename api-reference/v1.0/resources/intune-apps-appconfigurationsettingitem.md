---
title: appConfigurationSettingItem-Ressourcentyp
description: Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.
ms.openlocfilehash: bd08b325fd04e8e4a742da515d052d453cfb58a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017829"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="16eca-103">appConfigurationSettingItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16eca-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="16eca-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16eca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16eca-105">Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.</span><span class="sxs-lookup"><span data-stu-id="16eca-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="16eca-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16eca-106">Properties</span></span>
|<span data-ttu-id="16eca-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16eca-107">Property</span></span>|<span data-ttu-id="16eca-108">Typ</span><span class="sxs-lookup"><span data-stu-id="16eca-108">Type</span></span>|<span data-ttu-id="16eca-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16eca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16eca-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="16eca-110">appConfigKey</span></span>|<span data-ttu-id="16eca-111">String</span><span class="sxs-lookup"><span data-stu-id="16eca-111">String</span></span>|<span data-ttu-id="16eca-112">App-Konfigurationsschlüssel</span><span class="sxs-lookup"><span data-stu-id="16eca-112">app configuration key.</span></span>|
|<span data-ttu-id="16eca-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="16eca-113">appConfigKeyType</span></span>|[<span data-ttu-id="16eca-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="16eca-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="16eca-115">Typs des App-Konfigurationsschlüssels.</span><span class="sxs-lookup"><span data-stu-id="16eca-115">app configuration key type.</span></span> <span data-ttu-id="16eca-116">Mögliche Werte: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="16eca-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="16eca-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="16eca-117">appConfigKeyValue</span></span>|<span data-ttu-id="16eca-118">String</span><span class="sxs-lookup"><span data-stu-id="16eca-118">String</span></span>|<span data-ttu-id="16eca-119">Wert des App-Konfigurationsschlüssels</span><span class="sxs-lookup"><span data-stu-id="16eca-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16eca-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16eca-120">Relationships</span></span>
<span data-ttu-id="16eca-121">Keine</span><span class="sxs-lookup"><span data-stu-id="16eca-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="16eca-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16eca-122">JSON Representation</span></span>
<span data-ttu-id="16eca-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16eca-123">Here is a JSON representation of the resource.</span></span>
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



