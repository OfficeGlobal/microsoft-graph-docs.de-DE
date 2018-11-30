---
title: Ressourcentyp win32LobAppFileSystemDetection
description: Enthält Datei- oder Ordnerpfads zum Erkennen von einer Win32-App
ms.openlocfilehash: 914c4f550b480bf16b2048945e66542311653338
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064680"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="659e4-103">Ressourcentyp win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="659e4-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="659e4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="659e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="659e4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="659e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="659e4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="659e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="659e4-107">Enthält Datei- oder Ordnerpfads zum Erkennen von einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="659e4-107">Contains file or folder path to detect a Win32 App</span></span>

<span data-ttu-id="659e4-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="659e4-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="659e4-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="659e4-109">Properties</span></span>
|<span data-ttu-id="659e4-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="659e4-110">Property</span></span>|<span data-ttu-id="659e4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="659e4-111">Type</span></span>|<span data-ttu-id="659e4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="659e4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="659e4-113">Pfad</span><span class="sxs-lookup"><span data-stu-id="659e4-113">path</span></span>|<span data-ttu-id="659e4-114">String</span><span class="sxs-lookup"><span data-stu-id="659e4-114">String</span></span>|<span data-ttu-id="659e4-115">Der Datei- oder Ordnerpfads zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="659e4-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="659e4-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="659e4-116">fileOrFolderName</span></span>|<span data-ttu-id="659e4-117">String</span><span class="sxs-lookup"><span data-stu-id="659e4-117">String</span></span>|<span data-ttu-id="659e4-118">Der File- oder Folder Name zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="659e4-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="659e4-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="659e4-119">check32BitOn64System</span></span>|<span data-ttu-id="659e4-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="659e4-120">Boolean</span></span>|<span data-ttu-id="659e4-121">Ein Wert, der angibt, ob diese Datei oder eines Ordners ist für die Überprüfung auf 32-Bit-app auf 64-Bit-system</span><span class="sxs-lookup"><span data-stu-id="659e4-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="659e4-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="659e4-122">detectionType</span></span>|[<span data-ttu-id="659e4-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="659e4-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="659e4-124">Typ des Dateisystems Erkennung.</span><span class="sxs-lookup"><span data-stu-id="659e4-124">The file system detection type.</span></span> <span data-ttu-id="659e4-125">Mögliche Werte sind: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version` und `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="659e4-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="659e4-126">operator</span><span class="sxs-lookup"><span data-stu-id="659e4-126">operator</span></span>|[<span data-ttu-id="659e4-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="659e4-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="659e4-128">Der Operator für die Datei oder Fodler Erkennung.</span><span class="sxs-lookup"><span data-stu-id="659e4-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="659e4-129">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="659e4-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="659e4-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="659e4-130">detectionValue</span></span>|<span data-ttu-id="659e4-131">String</span><span class="sxs-lookup"><span data-stu-id="659e4-131">String</span></span>|<span data-ttu-id="659e4-132">Der Wert der Erkennung Datei oder eines Ordners</span><span class="sxs-lookup"><span data-stu-id="659e4-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="659e4-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="659e4-133">Relationships</span></span>
<span data-ttu-id="659e4-134">Keine</span><span class="sxs-lookup"><span data-stu-id="659e4-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="659e4-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="659e4-135">JSON Representation</span></span>
<span data-ttu-id="659e4-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="659e4-136">Here is a JSON representation of the resource.</span></span>
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





