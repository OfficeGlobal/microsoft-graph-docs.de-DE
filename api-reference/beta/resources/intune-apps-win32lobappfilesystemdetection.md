---
title: Ressourcentyp win32LobAppFileSystemDetection
description: Enthält Datei- oder Ordnerpfads zum Erkennen von einer Win32-App
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5fb4e66ce17fb7a964f3210244e2f3a7027c578
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415229"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="f4584-103">Ressourcentyp win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="f4584-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="f4584-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f4584-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4584-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4584-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4584-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f4584-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4584-107">Enthält Datei- oder Ordnerpfads zum Erkennen von einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="f4584-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="f4584-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="f4584-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f4584-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f4584-109">Properties</span></span>
|<span data-ttu-id="f4584-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4584-110">Property</span></span>|<span data-ttu-id="f4584-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f4584-111">Type</span></span>|<span data-ttu-id="f4584-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4584-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4584-113">Pfad</span><span class="sxs-lookup"><span data-stu-id="f4584-113">path</span></span>|<span data-ttu-id="f4584-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4584-114">String</span></span>|<span data-ttu-id="f4584-115">Der Datei- oder Ordnerpfads zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="f4584-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="f4584-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="f4584-116">fileOrFolderName</span></span>|<span data-ttu-id="f4584-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4584-117">String</span></span>|<span data-ttu-id="f4584-118">Der File- oder Folder Name zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="f4584-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="f4584-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="f4584-119">check32BitOn64System</span></span>|<span data-ttu-id="f4584-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4584-120">Boolean</span></span>|<span data-ttu-id="f4584-121">Ein Wert, der angibt, ob diese Datei oder eines Ordners ist für die Überprüfung auf 32-Bit-app auf 64-Bit-system</span><span class="sxs-lookup"><span data-stu-id="f4584-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="f4584-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="f4584-122">detectionType</span></span>|[<span data-ttu-id="f4584-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="f4584-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="f4584-124">Typ des Dateisystems Erkennung.</span><span class="sxs-lookup"><span data-stu-id="f4584-124">The file system detection type.</span></span> <span data-ttu-id="f4584-125">Mögliche Werte sind: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version` und `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="f4584-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="f4584-126">operator</span><span class="sxs-lookup"><span data-stu-id="f4584-126">operator</span></span>|[<span data-ttu-id="f4584-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="f4584-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="f4584-128">Der Operator für die Datei oder Fodler Erkennung.</span><span class="sxs-lookup"><span data-stu-id="f4584-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="f4584-129">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="f4584-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="f4584-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="f4584-130">detectionValue</span></span>|<span data-ttu-id="f4584-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4584-131">String</span></span>|<span data-ttu-id="f4584-132">Der Wert der Erkennung Datei oder eines Ordners</span><span class="sxs-lookup"><span data-stu-id="f4584-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4584-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f4584-133">Relationships</span></span>
<span data-ttu-id="f4584-134">Keine</span><span class="sxs-lookup"><span data-stu-id="f4584-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4584-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f4584-135">JSON Representation</span></span>
<span data-ttu-id="f4584-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f4584-136">Here is a JSON representation of the resource.</span></span>
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




