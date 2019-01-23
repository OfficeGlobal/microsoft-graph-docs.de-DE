---
title: Ressourcentyp win32LobAppPowerShellScriptDetection
description: Enthält Eigenschaften, die PowerShell-Skript zum Erkennen von einer Win32-App
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5c02228589042d0abf36c34c5818c5a4610514e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399640"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="cb60c-103">Ressourcentyp win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="cb60c-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="cb60c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cb60c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb60c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb60c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb60c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb60c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb60c-107">Enthält Eigenschaften, die PowerShell-Skript zum Erkennen von einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="cb60c-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="cb60c-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="cb60c-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb60c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb60c-109">Properties</span></span>
|<span data-ttu-id="cb60c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb60c-110">Property</span></span>|<span data-ttu-id="cb60c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="cb60c-111">Type</span></span>|<span data-ttu-id="cb60c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb60c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb60c-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="cb60c-113">enforceSignatureCheck</span></span>|<span data-ttu-id="cb60c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb60c-114">Boolean</span></span>|<span data-ttu-id="cb60c-115">Ein Wert, der angibt, ob die Signatur Kontrollkästchen erzwungen wird</span><span class="sxs-lookup"><span data-stu-id="cb60c-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="cb60c-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="cb60c-116">runAs32Bit</span></span>|<span data-ttu-id="cb60c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb60c-117">Boolean</span></span>|<span data-ttu-id="cb60c-118">Ein Wert, der angibt, ob dieses Skript als 32-Bit ausgeführt werden soll</span><span class="sxs-lookup"><span data-stu-id="cb60c-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="cb60c-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="cb60c-119">scriptContent</span></span>|<span data-ttu-id="cb60c-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb60c-120">String</span></span>|<span data-ttu-id="cb60c-121">Die base64-codierten Skriptinhalt zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="cb60c-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb60c-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cb60c-122">Relationships</span></span>
<span data-ttu-id="cb60c-123">Keine</span><span class="sxs-lookup"><span data-stu-id="cb60c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb60c-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb60c-124">JSON Representation</span></span>
<span data-ttu-id="cb60c-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb60c-125">Here is a JSON representation of the resource.</span></span>
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




