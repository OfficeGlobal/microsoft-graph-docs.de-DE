---
title: Ressourcentyp windowsKioskMultipleApps
description: Die Klasse verwendet, um die Konfiguration der Multi-Mode app für die Kiosk-Konfiguration identifizieren
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3770f8c63be230dff97e43d3706ed35d79826751
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977129"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="ddd1a-103">Ressourcentyp windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="ddd1a-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="ddd1a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddd1a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddd1a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddd1a-107">Die Klasse verwendet, um die Konfiguration der Multi-Mode app für die Kiosk-Konfiguration identifizieren</span><span class="sxs-lookup"><span data-stu-id="ddd1a-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="ddd1a-108">Erbt vom [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd1a-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ddd1a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ddd1a-109">Properties</span></span>
|<span data-ttu-id="ddd1a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ddd1a-110">Property</span></span>|<span data-ttu-id="ddd1a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ddd1a-111">Type</span></span>|<span data-ttu-id="ddd1a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ddd1a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd1a-113">Apps</span><span class="sxs-lookup"><span data-stu-id="ddd1a-113">apps</span></span>|<span data-ttu-id="ddd1a-114">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ddd1a-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="ddd1a-115">Dies sind die einzige Windows Store-Apps, die über das Startmenü gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="ddd1a-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="ddd1a-116">showTaskBar</span></span>|<span data-ttu-id="ddd1a-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ddd1a-117">Boolean</span></span>|<span data-ttu-id="ddd1a-118">Mit dieser Einstellung kann den Administrator an, ob der Taskleiste oder nicht angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="ddd1a-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="ddd1a-119">disallowDesktopApps</span></span>|<span data-ttu-id="ddd1a-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ddd1a-120">Boolean</span></span>|<span data-ttu-id="ddd1a-121">Diese Einstellung gibt an, dass desktop-apps zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="ddd1a-122">Standardmäßig auf "true".</span><span class="sxs-lookup"><span data-stu-id="ddd1a-122">Default to true.</span></span>|
|<span data-ttu-id="ddd1a-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="ddd1a-123">startMenuLayoutXml</span></span>|<span data-ttu-id="ddd1a-124">Binär</span><span class="sxs-lookup"><span data-stu-id="ddd1a-124">Binary</span></span>|<span data-ttu-id="ddd1a-125">Ermöglicht Administratoren das Standardlayout Start außer Kraft gesetzt, und verhindert, dass den Benutzer geändert wird.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="ddd1a-126">Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="ddd1a-127">XML muss im Binärformat sein.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddd1a-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ddd1a-128">Relationships</span></span>
<span data-ttu-id="ddd1a-129">Keine</span><span class="sxs-lookup"><span data-stu-id="ddd1a-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ddd1a-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ddd1a-130">JSON Representation</span></span>
<span data-ttu-id="ddd1a-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ddd1a-131">Here is a JSON representation of the resource.</span></span>
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





