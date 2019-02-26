---
title: win32LobAppFileSystemDetection-Ressourcentyp
description: Enthält Datei-oder Ordnerpfad zum Auffinden einer Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8145e6196b6537eec4142d4412a11234913df7c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157512"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="d99a6-103">win32LobAppFileSystemDetection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d99a6-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="d99a6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d99a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d99a6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d99a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d99a6-106">Enthält Datei-oder Ordnerpfad zum Auffinden einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="d99a6-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="d99a6-107">Erbt von [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="d99a6-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d99a6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d99a6-108">Properties</span></span>
|<span data-ttu-id="d99a6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d99a6-109">Property</span></span>|<span data-ttu-id="d99a6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d99a6-110">Type</span></span>|<span data-ttu-id="d99a6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d99a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d99a6-112">Pfad</span><span class="sxs-lookup"><span data-stu-id="d99a6-112">path</span></span>|<span data-ttu-id="d99a6-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d99a6-113">String</span></span>|<span data-ttu-id="d99a6-114">Der Datei-oder Ordnerpfad zur Ermittlung der Win32-Branchen-App</span><span class="sxs-lookup"><span data-stu-id="d99a6-114">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="d99a6-115">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="d99a6-115">fileOrFolderName</span></span>|<span data-ttu-id="d99a6-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d99a6-116">String</span></span>|<span data-ttu-id="d99a6-117">Der Datei-oder Ordnername zur Ermittlung der Win32-Branchen-App</span><span class="sxs-lookup"><span data-stu-id="d99a6-117">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="d99a6-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="d99a6-118">check32BitOn64System</span></span>|<span data-ttu-id="d99a6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d99a6-119">Boolean</span></span>|<span data-ttu-id="d99a6-120">Ein Wert, der angibt, ob diese Datei oder der Ordner zum Überprüfen der 32-Bit-App auf dem 64-Bit-System dient.</span><span class="sxs-lookup"><span data-stu-id="d99a6-120">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="d99a6-121">detectiontype</span><span class="sxs-lookup"><span data-stu-id="d99a6-121">detectionType</span></span>|[<span data-ttu-id="d99a6-122">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="d99a6-122">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="d99a6-123">Der Erkennungstyp des Dateisystems.</span><span class="sxs-lookup"><span data-stu-id="d99a6-123">The file system detection type.</span></span> <span data-ttu-id="d99a6-124">Mögliche Werte sind: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version` und `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="d99a6-124">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="d99a6-125">operator</span><span class="sxs-lookup"><span data-stu-id="d99a6-125">operator</span></span>|[<span data-ttu-id="d99a6-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="d99a6-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="d99a6-127">Der Operator für die Datei-oder fodler-Erkennung.</span><span class="sxs-lookup"><span data-stu-id="d99a6-127">The operator for file or fodler detection.</span></span> <span data-ttu-id="d99a6-128">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="d99a6-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="d99a6-129">Erkennungs-Value</span><span class="sxs-lookup"><span data-stu-id="d99a6-129">detectionValue</span></span>|<span data-ttu-id="d99a6-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d99a6-130">String</span></span>|<span data-ttu-id="d99a6-131">Der Wert für die Datei-oder Ordner Erkennung</span><span class="sxs-lookup"><span data-stu-id="d99a6-131">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d99a6-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d99a6-132">Relationships</span></span>
<span data-ttu-id="d99a6-133">Keine</span><span class="sxs-lookup"><span data-stu-id="d99a6-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d99a6-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d99a6-134">JSON Representation</span></span>
<span data-ttu-id="d99a6-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d99a6-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




