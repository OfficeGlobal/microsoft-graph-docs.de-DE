---
title: Ressourcentyp loggedOnUser
description: Angemeldete Benutzer
author: tfitzmac
ms.openlocfilehash: c2021d51356798dec906331797a2504f779264b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327174"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="d65c8-103">Ressourcentyp loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="d65c8-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="d65c8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d65c8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d65c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d65c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d65c8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d65c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d65c8-107">Angemeldete Benutzer</span><span class="sxs-lookup"><span data-stu-id="d65c8-107">Logged On User</span></span>
## <a name="properties"></a><span data-ttu-id="d65c8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d65c8-108">Properties</span></span>
|<span data-ttu-id="d65c8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d65c8-109">Property</span></span>|<span data-ttu-id="d65c8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d65c8-110">Type</span></span>|<span data-ttu-id="d65c8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d65c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d65c8-112">userId</span><span class="sxs-lookup"><span data-stu-id="d65c8-112">userId</span></span>|<span data-ttu-id="d65c8-113">String</span><span class="sxs-lookup"><span data-stu-id="d65c8-113">String</span></span>|<span data-ttu-id="d65c8-114">Benutzer-id</span><span class="sxs-lookup"><span data-stu-id="d65c8-114">User id</span></span>|
|<span data-ttu-id="d65c8-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="d65c8-115">lastLogOnDateTime</span></span>|<span data-ttu-id="d65c8-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d65c8-116">DateTimeOffset</span></span>|<span data-ttu-id="d65c8-117">Datum-Uhrzeit, wann Benutzer anmeldet</span><span class="sxs-lookup"><span data-stu-id="d65c8-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="d65c8-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d65c8-118">Relationships</span></span>
<span data-ttu-id="d65c8-119">Keine</span><span class="sxs-lookup"><span data-stu-id="d65c8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d65c8-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d65c8-120">JSON Representation</span></span>
<span data-ttu-id="d65c8-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d65c8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```





