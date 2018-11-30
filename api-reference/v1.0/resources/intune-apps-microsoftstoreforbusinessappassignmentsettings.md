---
title: microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp
description: Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.
ms.openlocfilehash: 62224841548c01ce84901251ab67204b82cbb4c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019980"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="5f27f-103">microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5f27f-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="5f27f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f27f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f27f-105">Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="5f27f-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="5f27f-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="5f27f-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5f27f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f27f-107">Properties</span></span>
|<span data-ttu-id="5f27f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f27f-108">Property</span></span>|<span data-ttu-id="5f27f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5f27f-109">Type</span></span>|<span data-ttu-id="5f27f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f27f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f27f-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="5f27f-111">useDeviceContext</span></span>|<span data-ttu-id="5f27f-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5f27f-112">Boolean</span></span>|<span data-ttu-id="5f27f-113">Gibt an, ob der Geräte-Ausführungskontext für mobile Microsoft Store für Unternehmen-Apps verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="5f27f-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f27f-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5f27f-114">Relationships</span></span>
<span data-ttu-id="5f27f-115">Keine</span><span class="sxs-lookup"><span data-stu-id="5f27f-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f27f-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f27f-116">JSON Representation</span></span>
<span data-ttu-id="5f27f-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5f27f-117">Here is a JSON representation of the resource.</span></span>
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


