---
title: Ressourcentyp androidPermissionAction
description: Zuordnung zwischen einer Android-app-Berechtigung und die Aktion Android sollte verwenden, wenn diese Berechtigung angefordert wird.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62355c3427083df09963e316f3b6b3c104a8662f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425631"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="2f90f-103">Ressourcentyp androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="2f90f-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="2f90f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2f90f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f90f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f90f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f90f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f90f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f90f-107">Zuordnung zwischen einer Android-app-Berechtigung und die Aktion Android sollte verwenden, wenn diese Berechtigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="2f90f-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="2f90f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2f90f-108">Properties</span></span>
|<span data-ttu-id="2f90f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f90f-109">Property</span></span>|<span data-ttu-id="2f90f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2f90f-110">Type</span></span>|<span data-ttu-id="2f90f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f90f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f90f-112">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="2f90f-112">permission</span></span>|<span data-ttu-id="2f90f-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f90f-113">String</span></span>|<span data-ttu-id="2f90f-114">In der Dokumentation zu offiziellen Android definierte Zeichenfolge Android Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="2f90f-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="2f90f-115">Beispiel für 'android.permission.READ_CONTACTS'.</span><span class="sxs-lookup"><span data-stu-id="2f90f-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="2f90f-116">Aktion</span><span class="sxs-lookup"><span data-stu-id="2f90f-116">action</span></span>|[<span data-ttu-id="2f90f-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="2f90f-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="2f90f-118">Typ der Berechtigung Android-Aktion.</span><span class="sxs-lookup"><span data-stu-id="2f90f-118">Type of Android permission action.</span></span> <span data-ttu-id="2f90f-119">Mögliche Werte sind: `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="2f90f-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f90f-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2f90f-120">Relationships</span></span>
<span data-ttu-id="2f90f-121">Keine</span><span class="sxs-lookup"><span data-stu-id="2f90f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f90f-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2f90f-122">JSON Representation</span></span>
<span data-ttu-id="2f90f-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2f90f-123">Here is a JSON representation of the resource.</span></span>
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




