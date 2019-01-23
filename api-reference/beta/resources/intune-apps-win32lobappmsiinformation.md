---
title: Ressourcentyp win32LobAppMsiInformation
description: Enthält die MSI-app-Eigenschaften für eine Win32-App.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ba91c572286020a3e349527f325d22bf0be5d67
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399248"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="c9b7e-103">Ressourcentyp win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="c9b7e-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="c9b7e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c9b7e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9b7e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9b7e-107">Enthält die MSI-app-Eigenschaften für eine Win32-App.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="c9b7e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9b7e-108">Properties</span></span>
|<span data-ttu-id="c9b7e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9b7e-109">Property</span></span>|<span data-ttu-id="c9b7e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c9b7e-110">Type</span></span>|<span data-ttu-id="c9b7e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9b7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9b7e-112">productCode</span><span class="sxs-lookup"><span data-stu-id="c9b7e-112">productCode</span></span>|<span data-ttu-id="c9b7e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9b7e-113">String</span></span>|<span data-ttu-id="c9b7e-114">Der MSI-Produktcode.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-114">The MSI product code.</span></span>|
|<span data-ttu-id="c9b7e-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="c9b7e-115">productVersion</span></span>|<span data-ttu-id="c9b7e-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9b7e-116">String</span></span>|<span data-ttu-id="c9b7e-117">Der MSI-Version des Produkts.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-117">The MSI product version.</span></span>|
|<span data-ttu-id="c9b7e-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="c9b7e-118">upgradeCode</span></span>|<span data-ttu-id="c9b7e-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9b7e-119">String</span></span>|<span data-ttu-id="c9b7e-120">Die MSI-Datei aktualisieren von Code.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="c9b7e-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="c9b7e-121">requiresReboot</span></span>|<span data-ttu-id="c9b7e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b7e-122">Boolean</span></span>|<span data-ttu-id="c9b7e-123">Gibt an, ob erfordert die MSI-app für den Computer neu starten, um die Installation abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="c9b7e-124">packageType</span><span class="sxs-lookup"><span data-stu-id="c9b7e-124">packageType</span></span>|[<span data-ttu-id="c9b7e-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="c9b7e-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="c9b7e-126">Der Typ des MSI-Paket.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-126">The MSI package type.</span></span> <span data-ttu-id="c9b7e-127">Mögliche Werte sind: `perMachine`, `perUser` und `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9b7e-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c9b7e-128">Relationships</span></span>
<span data-ttu-id="c9b7e-129">Keine</span><span class="sxs-lookup"><span data-stu-id="c9b7e-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9b7e-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9b7e-130">JSON Representation</span></span>
<span data-ttu-id="c9b7e-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9b7e-131">Here is a JSON representation of the resource.</span></span>
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




