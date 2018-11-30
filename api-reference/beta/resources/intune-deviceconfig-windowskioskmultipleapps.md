---
title: Ressourcentyp windowsKioskMultipleApps
description: Die Klasse verwendet, um die Konfiguration der Multi-Mode app für die Kiosk-Konfiguration identifizieren
ms.openlocfilehash: 2b52cbe343c4a8d81391ad448e8f10f64fef295e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060782"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="80a04-103">Ressourcentyp windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="80a04-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="80a04-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80a04-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80a04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80a04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80a04-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80a04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80a04-107">Die Klasse verwendet, um die Konfiguration der Multi-Mode app für die Kiosk-Konfiguration identifizieren</span><span class="sxs-lookup"><span data-stu-id="80a04-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="80a04-108">Erbt vom [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80a04-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80a04-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80a04-109">Properties</span></span>
|<span data-ttu-id="80a04-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80a04-110">Property</span></span>|<span data-ttu-id="80a04-111">Typ</span><span class="sxs-lookup"><span data-stu-id="80a04-111">Type</span></span>|<span data-ttu-id="80a04-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80a04-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80a04-113">Apps</span><span class="sxs-lookup"><span data-stu-id="80a04-113">apps</span></span>|<span data-ttu-id="80a04-114">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="80a04-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="80a04-115">Dies sind die einzige Windows Store-Apps, die über das Startmenü gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="80a04-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="80a04-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="80a04-116">showTaskBar</span></span>|<span data-ttu-id="80a04-117">Boolesch</span><span class="sxs-lookup"><span data-stu-id="80a04-117">Boolean</span></span>|<span data-ttu-id="80a04-118">Mit dieser Einstellung kann den Administrator an, ob der Taskleiste oder nicht angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="80a04-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="80a04-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="80a04-119">disallowDesktopApps</span></span>|<span data-ttu-id="80a04-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="80a04-120">Boolean</span></span>|<span data-ttu-id="80a04-121">Diese Einstellung gibt an, dass desktop-apps zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="80a04-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="80a04-122">Standardmäßig auf "true".</span><span class="sxs-lookup"><span data-stu-id="80a04-122">Default to true.</span></span>|
|<span data-ttu-id="80a04-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="80a04-123">startMenuLayoutXml</span></span>|<span data-ttu-id="80a04-124">Binär</span><span class="sxs-lookup"><span data-stu-id="80a04-124">Binary</span></span>|<span data-ttu-id="80a04-125">Ermöglicht Administratoren das Standardlayout Start außer Kraft gesetzt, und verhindert, dass den Benutzer geändert wird.</span><span class="sxs-lookup"><span data-stu-id="80a04-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="80a04-126">Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert.</span><span class="sxs-lookup"><span data-stu-id="80a04-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="80a04-127">XML muss im Binärformat sein.</span><span class="sxs-lookup"><span data-stu-id="80a04-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80a04-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="80a04-128">Relationships</span></span>
<span data-ttu-id="80a04-129">Keine</span><span class="sxs-lookup"><span data-stu-id="80a04-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80a04-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80a04-130">JSON Representation</span></span>
<span data-ttu-id="80a04-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80a04-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





