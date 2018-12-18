---
title: microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp
description: Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.
author: tfitzmac
ms.openlocfilehash: 3a6d33eac4ee03a54e99a24cfde3b15c82cb0bad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342910"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="f8f3d-103">microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8f3d-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f8f3d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f8f3d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8f3d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8f3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8f3d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f8f3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8f3d-107">Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="f8f3d-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="f8f3d-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f8f3d-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8f3d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8f3d-109">Properties</span></span>
|<span data-ttu-id="f8f3d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8f3d-110">Property</span></span>|<span data-ttu-id="f8f3d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f8f3d-111">Type</span></span>|<span data-ttu-id="f8f3d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8f3d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8f3d-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="f8f3d-113">useDeviceContext</span></span>|<span data-ttu-id="f8f3d-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f8f3d-114">Boolean</span></span>|<span data-ttu-id="f8f3d-115">Gibt an, ob der Geräte-Ausführungskontext für mobile Microsoft Store für Unternehmen-Apps verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="f8f3d-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8f3d-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f8f3d-116">Relationships</span></span>
<span data-ttu-id="f8f3d-117">Keine</span><span class="sxs-lookup"><span data-stu-id="f8f3d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8f3d-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8f3d-118">JSON Representation</span></span>
<span data-ttu-id="f8f3d-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8f3d-119">Here is a JSON representation of the resource.</span></span>
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





