---
title: Ressourcentyp androidPermissionAction
description: Zuordnung zwischen einer Android-app-Berechtigung und die Aktion Android sollte verwenden, wenn diese Berechtigung angefordert wird.
author: tfitzmac
ms.openlocfilehash: 90117b30dae765151e79d8ad1c2ae1afaa5a42ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331136"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="9ec72-103">Ressourcentyp androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="9ec72-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="9ec72-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9ec72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ec72-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ec72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ec72-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9ec72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ec72-107">Zuordnung zwischen einer Android-app-Berechtigung und die Aktion Android sollte verwenden, wenn diese Berechtigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="9ec72-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="9ec72-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9ec72-108">Properties</span></span>
|<span data-ttu-id="9ec72-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ec72-109">Property</span></span>|<span data-ttu-id="9ec72-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9ec72-110">Type</span></span>|<span data-ttu-id="9ec72-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ec72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec72-112">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="9ec72-112">permission</span></span>|<span data-ttu-id="9ec72-113">String</span><span class="sxs-lookup"><span data-stu-id="9ec72-113">String</span></span>|<span data-ttu-id="9ec72-114">In der Dokumentation zu offiziellen Android definierte Zeichenfolge Android Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="9ec72-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="9ec72-115">Beispiel für 'android.permission.READ_CONTACTS'.</span><span class="sxs-lookup"><span data-stu-id="9ec72-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="9ec72-116">Aktion</span><span class="sxs-lookup"><span data-stu-id="9ec72-116">action</span></span>|[<span data-ttu-id="9ec72-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="9ec72-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="9ec72-118">Typ der Berechtigung Android-Aktion.</span><span class="sxs-lookup"><span data-stu-id="9ec72-118">Type of Android permission action.</span></span> <span data-ttu-id="9ec72-119">Mögliche Werte sind: `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="9ec72-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ec72-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9ec72-120">Relationships</span></span>
<span data-ttu-id="9ec72-121">Keine</span><span class="sxs-lookup"><span data-stu-id="9ec72-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ec72-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9ec72-122">JSON Representation</span></span>
<span data-ttu-id="9ec72-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9ec72-123">Here is a JSON representation of the resource.</span></span>
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





