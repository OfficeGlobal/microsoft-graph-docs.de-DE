---
title: androidPermissionAction-Ressourcentyp
description: Zuordnung zwischen einer Android-App-Berechtigung und der Aktion, die Android ausführen sollte, wenn diese Berechtigung angefordert wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e00bb351f2eff093dee21cb393ba622bc5e29ea9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161572"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="091e9-103">androidPermissionAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="091e9-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="091e9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="091e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="091e9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="091e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="091e9-106">Zuordnung zwischen einer Android-App-Berechtigung und der Aktion, die Android ausführen sollte, wenn diese Berechtigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="091e9-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="091e9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="091e9-107">Properties</span></span>
|<span data-ttu-id="091e9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="091e9-108">Property</span></span>|<span data-ttu-id="091e9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="091e9-109">Type</span></span>|<span data-ttu-id="091e9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="091e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="091e9-111">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="091e9-111">permission</span></span>|<span data-ttu-id="091e9-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="091e9-112">String</span></span>|<span data-ttu-id="091e9-113">Android-Berechtigungszeichenfolge, definiert in der offiziellen Android-Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="091e9-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="091e9-114">Beispiel "Android. Permission. READ_CONTACTS".</span><span class="sxs-lookup"><span data-stu-id="091e9-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="091e9-115">Aktion</span><span class="sxs-lookup"><span data-stu-id="091e9-115">action</span></span>|[<span data-ttu-id="091e9-116">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="091e9-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="091e9-117">Typ der Android-Berechtigungs Aktion.</span><span class="sxs-lookup"><span data-stu-id="091e9-117">Type of Android permission action.</span></span> <span data-ttu-id="091e9-118">Mögliche Werte sind: `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="091e9-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="091e9-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="091e9-119">Relationships</span></span>
<span data-ttu-id="091e9-120">Keine</span><span class="sxs-lookup"><span data-stu-id="091e9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="091e9-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="091e9-121">JSON Representation</span></span>
<span data-ttu-id="091e9-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="091e9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```




