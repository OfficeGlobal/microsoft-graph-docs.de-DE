---
title: win32LobAppPowerShellScriptDetection-Ressourcentyp
description: Enthält PowerShell-Skripteigenschaften zum Auffinden einer Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa5452fd9e73aef846d0b6de86a2b84e2c42ba26
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168523"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="594bd-103">win32LobAppPowerShellScriptDetection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="594bd-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="594bd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="594bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="594bd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="594bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="594bd-106">Enthält PowerShell-Skripteigenschaften zum Auffinden einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="594bd-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="594bd-107">Erbt von [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="594bd-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="594bd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="594bd-108">Properties</span></span>
|<span data-ttu-id="594bd-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="594bd-109">Property</span></span>|<span data-ttu-id="594bd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="594bd-110">Type</span></span>|<span data-ttu-id="594bd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="594bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="594bd-112">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="594bd-112">enforceSignatureCheck</span></span>|<span data-ttu-id="594bd-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="594bd-113">Boolean</span></span>|<span data-ttu-id="594bd-114">Ein Wert, der angibt, ob die Signaturüberprüfung erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="594bd-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="594bd-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="594bd-115">runAs32Bit</span></span>|<span data-ttu-id="594bd-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="594bd-116">Boolean</span></span>|<span data-ttu-id="594bd-117">Ein Wert, der angibt, ob dieses Skript als 32-Bit ausgeführt werden soll</span><span class="sxs-lookup"><span data-stu-id="594bd-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="594bd-118">scriptContent</span><span class="sxs-lookup"><span data-stu-id="594bd-118">scriptContent</span></span>|<span data-ttu-id="594bd-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="594bd-119">String</span></span>|<span data-ttu-id="594bd-120">Der Base64-codierte Skriptinhalt zum Aufspüren der Win32-Branchen-App</span><span class="sxs-lookup"><span data-stu-id="594bd-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="594bd-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="594bd-121">Relationships</span></span>
<span data-ttu-id="594bd-122">Keine</span><span class="sxs-lookup"><span data-stu-id="594bd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="594bd-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="594bd-123">JSON Representation</span></span>
<span data-ttu-id="594bd-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="594bd-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```




