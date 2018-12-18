---
title: Ressourcentyp macOSLobChildApp
description: Enthält Eigenschaften, die die Mac OS LOB-App in einem Paket bundle
author: tfitzmac
ms.openlocfilehash: e62305ea856d42847b49be306d20bde737152163
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309870"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="3edac-103">Ressourcentyp macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="3edac-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="3edac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3edac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3edac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3edac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3edac-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3edac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3edac-107">Enthält Eigenschaften, die die Mac OS LOB-App in einem Paket bundle</span><span class="sxs-lookup"><span data-stu-id="3edac-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="3edac-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3edac-108">Properties</span></span>
|<span data-ttu-id="3edac-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3edac-109">Property</span></span>|<span data-ttu-id="3edac-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3edac-110">Type</span></span>|<span data-ttu-id="3edac-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3edac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3edac-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="3edac-112">bundleId</span></span>|<span data-ttu-id="3edac-113">String</span><span class="sxs-lookup"><span data-stu-id="3edac-113">String</span></span>|<span data-ttu-id="3edac-114">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="3edac-114">The Identity Name.</span></span>|
|<span data-ttu-id="3edac-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="3edac-115">buildNumber</span></span>|<span data-ttu-id="3edac-116">String</span><span class="sxs-lookup"><span data-stu-id="3edac-116">String</span></span>|<span data-ttu-id="3edac-117">Die Buildnummer der Mac OS-Zeile des Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="3edac-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3edac-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="3edac-118">versionNumber</span></span>|<span data-ttu-id="3edac-119">String</span><span class="sxs-lookup"><span data-stu-id="3edac-119">String</span></span>|<span data-ttu-id="3edac-120">Die Versionsnummer der Mac OS-Zeile des Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="3edac-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3edac-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3edac-121">Relationships</span></span>
<span data-ttu-id="3edac-122">Keine</span><span class="sxs-lookup"><span data-stu-id="3edac-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3edac-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3edac-123">JSON Representation</span></span>
<span data-ttu-id="3edac-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3edac-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





