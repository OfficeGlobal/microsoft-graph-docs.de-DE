---
title: Ressourcentyp win32LobAppPowerShellScriptDetection
description: Enthält Eigenschaften, die PowerShell-Skript zum Erkennen von einer Win32-App
ms.openlocfilehash: e5d87d3d2a90c0ac7f8ce6db7e14b105583a76f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061957"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="003a3-103">Ressourcentyp win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="003a3-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="003a3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="003a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="003a3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="003a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="003a3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="003a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="003a3-107">Enthält Eigenschaften, die PowerShell-Skript zum Erkennen von einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="003a3-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="003a3-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="003a3-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="003a3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="003a3-109">Properties</span></span>
|<span data-ttu-id="003a3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="003a3-110">Property</span></span>|<span data-ttu-id="003a3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="003a3-111">Type</span></span>|<span data-ttu-id="003a3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="003a3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="003a3-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="003a3-113">enforceSignatureCheck</span></span>|<span data-ttu-id="003a3-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="003a3-114">Boolean</span></span>|<span data-ttu-id="003a3-115">Ein Wert, der angibt, ob die Signatur Kontrollkästchen erzwungen wird</span><span class="sxs-lookup"><span data-stu-id="003a3-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="003a3-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="003a3-116">runAs32Bit</span></span>|<span data-ttu-id="003a3-117">Boolesch</span><span class="sxs-lookup"><span data-stu-id="003a3-117">Boolean</span></span>|<span data-ttu-id="003a3-118">Ein Wert, der angibt, ob dieses Skript als 32-Bit ausgeführt werden soll</span><span class="sxs-lookup"><span data-stu-id="003a3-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="003a3-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="003a3-119">scriptContent</span></span>|<span data-ttu-id="003a3-120">String</span><span class="sxs-lookup"><span data-stu-id="003a3-120">String</span></span>|<span data-ttu-id="003a3-121">Die base64-codierten Skriptinhalt zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="003a3-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="003a3-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="003a3-122">Relationships</span></span>
<span data-ttu-id="003a3-123">Keine</span><span class="sxs-lookup"><span data-stu-id="003a3-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="003a3-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="003a3-124">JSON Representation</span></span>
<span data-ttu-id="003a3-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="003a3-125">Here is a JSON representation of the resource.</span></span>
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





