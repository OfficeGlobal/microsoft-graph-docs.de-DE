---
title: microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp
description: Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1aed45ba54abdcb25f5436beeb2a03f53b9dbae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261103"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="99df0-103">microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="99df0-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="99df0-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="99df0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99df0-105">Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="99df0-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="99df0-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="99df0-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99df0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="99df0-107">Properties</span></span>
|<span data-ttu-id="99df0-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99df0-108">Property</span></span>|<span data-ttu-id="99df0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="99df0-109">Type</span></span>|<span data-ttu-id="99df0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99df0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99df0-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="99df0-111">useDeviceContext</span></span>|<span data-ttu-id="99df0-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="99df0-112">Boolean</span></span>|<span data-ttu-id="99df0-113">Gibt an, ob der Geräte-Ausführungskontext für mobile Microsoft Store für Unternehmen-Apps verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="99df0-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99df0-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="99df0-114">Relationships</span></span>
<span data-ttu-id="99df0-115">Keine</span><span class="sxs-lookup"><span data-stu-id="99df0-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99df0-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="99df0-116">JSON Representation</span></span>
<span data-ttu-id="99df0-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="99df0-117">Here is a JSON representation of the resource.</span></span>
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



