---
title: microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp
description: Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5f566a04169be20777b9f0fb5a7aa911ad3e864
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393249"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="a8b31-103">microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a8b31-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a8b31-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a8b31-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8b31-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8b31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8b31-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8b31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8b31-107">Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="a8b31-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="a8b31-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a8b31-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8b31-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8b31-109">Properties</span></span>
|<span data-ttu-id="a8b31-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8b31-110">Property</span></span>|<span data-ttu-id="a8b31-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a8b31-111">Type</span></span>|<span data-ttu-id="a8b31-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8b31-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b31-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a8b31-113">useDeviceContext</span></span>|<span data-ttu-id="a8b31-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a8b31-114">Boolean</span></span>|<span data-ttu-id="a8b31-115">Gibt an, ob der Geräte-Ausführungskontext für mobile Microsoft Store für Unternehmen-Apps verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="a8b31-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8b31-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a8b31-116">Relationships</span></span>
<span data-ttu-id="a8b31-117">Keine</span><span class="sxs-lookup"><span data-stu-id="a8b31-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8b31-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8b31-118">JSON Representation</span></span>
<span data-ttu-id="a8b31-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8b31-119">Here is a JSON representation of the resource.</span></span>
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




