---
title: microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp
description: Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86922fa8b9ca587f0c777bbaed4b479620e6af21
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876370"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="5aa6d-103">microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5aa6d-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="5aa6d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5aa6d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5aa6d-105">Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="5aa6d-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="5aa6d-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="5aa6d-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5aa6d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5aa6d-107">Properties</span></span>
|<span data-ttu-id="5aa6d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5aa6d-108">Property</span></span>|<span data-ttu-id="5aa6d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5aa6d-109">Type</span></span>|<span data-ttu-id="5aa6d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5aa6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aa6d-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="5aa6d-111">useDeviceContext</span></span>|<span data-ttu-id="5aa6d-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5aa6d-112">Boolean</span></span>|<span data-ttu-id="5aa6d-113">Gibt an, ob der Geräte-Ausführungskontext für mobile Microsoft Store für Unternehmen-Apps verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="5aa6d-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5aa6d-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5aa6d-114">Relationships</span></span>
<span data-ttu-id="5aa6d-115">Keine</span><span class="sxs-lookup"><span data-stu-id="5aa6d-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5aa6d-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5aa6d-116">JSON Representation</span></span>
<span data-ttu-id="5aa6d-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5aa6d-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```



