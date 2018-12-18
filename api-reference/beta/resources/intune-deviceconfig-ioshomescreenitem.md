---
title: iosHomeScreenItem-Ressourcentyp
description: Stellt ein Element auf dem iOS-Startbildschirm dar.
author: tfitzmac
ms.openlocfilehash: 6a8d71e01ca8f2c284bcc3eddd7eb39b87c025d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328189"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="9be83-103">iosHomeScreenItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9be83-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="9be83-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9be83-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9be83-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9be83-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9be83-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9be83-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9be83-107">Stellt ein Element auf dem iOS-Startbildschirm dar.</span><span class="sxs-lookup"><span data-stu-id="9be83-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="9be83-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9be83-108">Properties</span></span>
|<span data-ttu-id="9be83-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9be83-109">Property</span></span>|<span data-ttu-id="9be83-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9be83-110">Type</span></span>|<span data-ttu-id="9be83-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9be83-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9be83-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9be83-112">displayName</span></span>|<span data-ttu-id="9be83-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9be83-113">String</span></span>|<span data-ttu-id="9be83-114">Name der App</span><span class="sxs-lookup"><span data-stu-id="9be83-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="9be83-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9be83-115">Relationships</span></span>
<span data-ttu-id="9be83-116">Keine</span><span class="sxs-lookup"><span data-stu-id="9be83-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9be83-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9be83-117">JSON Representation</span></span>
<span data-ttu-id="9be83-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9be83-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





