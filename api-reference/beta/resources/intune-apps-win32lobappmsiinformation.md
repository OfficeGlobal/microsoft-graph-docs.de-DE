---
title: win32LobAppMsiInformation-Ressourcentyp
description: Enthält Eigenschaften der MSI-App für eine Win32-app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f330111a3e924e54cf23c30cd98d20e85cb38022
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158646"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="ba096-103">win32LobAppMsiInformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ba096-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="ba096-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba096-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba096-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ba096-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba096-106">Enthält Eigenschaften der MSI-App für eine Win32-app.</span><span class="sxs-lookup"><span data-stu-id="ba096-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="ba096-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ba096-107">Properties</span></span>
|<span data-ttu-id="ba096-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba096-108">Property</span></span>|<span data-ttu-id="ba096-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ba096-109">Type</span></span>|<span data-ttu-id="ba096-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba096-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba096-111">productCode</span><span class="sxs-lookup"><span data-stu-id="ba096-111">productCode</span></span>|<span data-ttu-id="ba096-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba096-112">String</span></span>|<span data-ttu-id="ba096-113">Der MSI-Produktcode.</span><span class="sxs-lookup"><span data-stu-id="ba096-113">The MSI product code.</span></span>|
|<span data-ttu-id="ba096-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="ba096-114">productVersion</span></span>|<span data-ttu-id="ba096-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba096-115">String</span></span>|<span data-ttu-id="ba096-116">Die MSI-Produktversion.</span><span class="sxs-lookup"><span data-stu-id="ba096-116">The MSI product version.</span></span>|
|<span data-ttu-id="ba096-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="ba096-117">upgradeCode</span></span>|<span data-ttu-id="ba096-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba096-118">String</span></span>|<span data-ttu-id="ba096-119">Der MSI-UpgradeCode.</span><span class="sxs-lookup"><span data-stu-id="ba096-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="ba096-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="ba096-120">requiresReboot</span></span>|<span data-ttu-id="ba096-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba096-121">Boolean</span></span>|<span data-ttu-id="ba096-122">Gibt an, ob für die MSI-App der Computer neu gestartet werden muss, um die Installation abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="ba096-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="ba096-123">PackageType</span><span class="sxs-lookup"><span data-stu-id="ba096-123">packageType</span></span>|[<span data-ttu-id="ba096-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="ba096-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="ba096-125">Der MSI-Pakettyp.</span><span class="sxs-lookup"><span data-stu-id="ba096-125">The MSI package type.</span></span> <span data-ttu-id="ba096-126">Mögliche Werte sind: `perMachine`, `perUser` und `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="ba096-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="ba096-127">productName</span><span class="sxs-lookup"><span data-stu-id="ba096-127">productName</span></span>|<span data-ttu-id="ba096-128">String</span><span class="sxs-lookup"><span data-stu-id="ba096-128">String</span></span>|<span data-ttu-id="ba096-129">Der MSI-Produktname.</span><span class="sxs-lookup"><span data-stu-id="ba096-129">The MSI product name.</span></span>|
|<span data-ttu-id="ba096-130">publisher</span><span class="sxs-lookup"><span data-stu-id="ba096-130">publisher</span></span>|<span data-ttu-id="ba096-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba096-131">String</span></span>|<span data-ttu-id="ba096-132">Der MSI-Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="ba096-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba096-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ba096-133">Relationships</span></span>
<span data-ttu-id="ba096-134">Keine</span><span class="sxs-lookup"><span data-stu-id="ba096-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba096-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ba096-135">JSON Representation</span></span>
<span data-ttu-id="ba096-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ba096-136">Here is a JSON representation of the resource.</span></span>
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
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```




