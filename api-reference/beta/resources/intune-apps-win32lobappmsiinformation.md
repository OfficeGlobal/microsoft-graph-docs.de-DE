---
title: Ressourcentyp win32LobAppMsiInformation
description: Enthält die MSI-app-Eigenschaften für eine Win32-App.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04972e9e7fa909c220fe55ca6337be3ac44138ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967875"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="08b93-103">Ressourcentyp win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="08b93-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="08b93-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08b93-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08b93-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08b93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08b93-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="08b93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08b93-107">Enthält die MSI-app-Eigenschaften für eine Win32-App.</span><span class="sxs-lookup"><span data-stu-id="08b93-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="08b93-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08b93-108">Properties</span></span>
|<span data-ttu-id="08b93-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08b93-109">Property</span></span>|<span data-ttu-id="08b93-110">Typ</span><span class="sxs-lookup"><span data-stu-id="08b93-110">Type</span></span>|<span data-ttu-id="08b93-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08b93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08b93-112">productCode</span><span class="sxs-lookup"><span data-stu-id="08b93-112">productCode</span></span>|<span data-ttu-id="08b93-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08b93-113">String</span></span>|<span data-ttu-id="08b93-114">Der MSI-Produktcode.</span><span class="sxs-lookup"><span data-stu-id="08b93-114">The MSI product code.</span></span>|
|<span data-ttu-id="08b93-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="08b93-115">productVersion</span></span>|<span data-ttu-id="08b93-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08b93-116">String</span></span>|<span data-ttu-id="08b93-117">Der MSI-Version des Produkts.</span><span class="sxs-lookup"><span data-stu-id="08b93-117">The MSI product version.</span></span>|
|<span data-ttu-id="08b93-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="08b93-118">upgradeCode</span></span>|<span data-ttu-id="08b93-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08b93-119">String</span></span>|<span data-ttu-id="08b93-120">Die MSI-Datei aktualisieren von Code.</span><span class="sxs-lookup"><span data-stu-id="08b93-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="08b93-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="08b93-121">requiresReboot</span></span>|<span data-ttu-id="08b93-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08b93-122">Boolean</span></span>|<span data-ttu-id="08b93-123">Gibt an, ob erfordert die MSI-app für den Computer neu starten, um die Installation abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="08b93-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="08b93-124">packageType</span><span class="sxs-lookup"><span data-stu-id="08b93-124">packageType</span></span>|[<span data-ttu-id="08b93-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="08b93-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="08b93-126">Der Typ des MSI-Paket.</span><span class="sxs-lookup"><span data-stu-id="08b93-126">The MSI package type.</span></span> <span data-ttu-id="08b93-127">Mögliche Werte sind: `perMachine`, `perUser` und `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="08b93-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08b93-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08b93-128">Relationships</span></span>
<span data-ttu-id="08b93-129">Keine</span><span class="sxs-lookup"><span data-stu-id="08b93-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08b93-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08b93-130">JSON Representation</span></span>
<span data-ttu-id="08b93-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08b93-131">Here is a JSON representation of the resource.</span></span>
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





