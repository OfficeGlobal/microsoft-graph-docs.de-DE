---
title: Ressourcentyp win32LobAppPowerShellScriptDetection
description: Enthält Eigenschaften, die PowerShell-Skript zum Erkennen von einer Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38a3df87ca5492b89000fc1090395d94c64e1888
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926967"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="34418-103">Ressourcentyp win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="34418-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="34418-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34418-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34418-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34418-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34418-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="34418-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34418-107">Enthält Eigenschaften, die PowerShell-Skript zum Erkennen von einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="34418-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="34418-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="34418-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34418-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34418-109">Properties</span></span>
|<span data-ttu-id="34418-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34418-110">Property</span></span>|<span data-ttu-id="34418-111">Typ</span><span class="sxs-lookup"><span data-stu-id="34418-111">Type</span></span>|<span data-ttu-id="34418-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34418-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34418-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="34418-113">enforceSignatureCheck</span></span>|<span data-ttu-id="34418-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34418-114">Boolean</span></span>|<span data-ttu-id="34418-115">Ein Wert, der angibt, ob die Signatur Kontrollkästchen erzwungen wird</span><span class="sxs-lookup"><span data-stu-id="34418-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="34418-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="34418-116">runAs32Bit</span></span>|<span data-ttu-id="34418-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="34418-117">Boolean</span></span>|<span data-ttu-id="34418-118">Ein Wert, der angibt, ob dieses Skript als 32-Bit ausgeführt werden soll</span><span class="sxs-lookup"><span data-stu-id="34418-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="34418-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="34418-119">scriptContent</span></span>|<span data-ttu-id="34418-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34418-120">String</span></span>|<span data-ttu-id="34418-121">Die base64-codierten Skriptinhalt zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="34418-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="34418-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="34418-122">Relationships</span></span>
<span data-ttu-id="34418-123">Keine</span><span class="sxs-lookup"><span data-stu-id="34418-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="34418-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="34418-124">JSON Representation</span></span>
<span data-ttu-id="34418-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="34418-125">Here is a JSON representation of the resource.</span></span>
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





