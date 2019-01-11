---
title: Ressourcentyp win32LobAppMsiInformation
description: Enthält die MSI-app-Eigenschaften für eine Win32-App.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e43b3dc9e46ed193b7547a7ce85863253445d30c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846515"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="c75bd-103">Ressourcentyp win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="c75bd-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="c75bd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c75bd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c75bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c75bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c75bd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c75bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c75bd-107">Enthält die MSI-app-Eigenschaften für eine Win32-App.</span><span class="sxs-lookup"><span data-stu-id="c75bd-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="c75bd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c75bd-108">Properties</span></span>
|<span data-ttu-id="c75bd-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c75bd-109">Property</span></span>|<span data-ttu-id="c75bd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c75bd-110">Type</span></span>|<span data-ttu-id="c75bd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c75bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c75bd-112">productCode</span><span class="sxs-lookup"><span data-stu-id="c75bd-112">productCode</span></span>|<span data-ttu-id="c75bd-113">String</span><span class="sxs-lookup"><span data-stu-id="c75bd-113">String</span></span>|<span data-ttu-id="c75bd-114">Der MSI-Produktcode.</span><span class="sxs-lookup"><span data-stu-id="c75bd-114">The MSI product code.</span></span>|
|<span data-ttu-id="c75bd-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="c75bd-115">productVersion</span></span>|<span data-ttu-id="c75bd-116">String</span><span class="sxs-lookup"><span data-stu-id="c75bd-116">String</span></span>|<span data-ttu-id="c75bd-117">Der MSI-Version des Produkts.</span><span class="sxs-lookup"><span data-stu-id="c75bd-117">The MSI product version.</span></span>|
|<span data-ttu-id="c75bd-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="c75bd-118">upgradeCode</span></span>|<span data-ttu-id="c75bd-119">String</span><span class="sxs-lookup"><span data-stu-id="c75bd-119">String</span></span>|<span data-ttu-id="c75bd-120">Die MSI-Datei aktualisieren von Code.</span><span class="sxs-lookup"><span data-stu-id="c75bd-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="c75bd-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="c75bd-121">requiresReboot</span></span>|<span data-ttu-id="c75bd-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="c75bd-122">Boolean</span></span>|<span data-ttu-id="c75bd-123">Gibt an, ob erfordert die MSI-app für den Computer neu starten, um die Installation abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="c75bd-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="c75bd-124">packageType</span><span class="sxs-lookup"><span data-stu-id="c75bd-124">packageType</span></span>|[<span data-ttu-id="c75bd-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="c75bd-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="c75bd-126">Der Typ des MSI-Paket.</span><span class="sxs-lookup"><span data-stu-id="c75bd-126">The MSI package type.</span></span> <span data-ttu-id="c75bd-127">Mögliche Werte sind: `perMachine`, `perUser` und `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="c75bd-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c75bd-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c75bd-128">Relationships</span></span>
<span data-ttu-id="c75bd-129">Keine</span><span class="sxs-lookup"><span data-stu-id="c75bd-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c75bd-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c75bd-130">JSON Representation</span></span>
<span data-ttu-id="c75bd-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c75bd-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String"
}
```





