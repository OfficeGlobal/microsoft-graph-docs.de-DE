---
title: Ressourcentyp windowsKioskMultipleApps
description: Die Klasse verwendet, um die Konfiguration der Multi-Mode app für die Kiosk-Konfiguration identifizieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71b8a57151b08d0297a89dfd815f72d66c2d12a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396028"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="bd4c2-103">Ressourcentyp windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="bd4c2-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="bd4c2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd4c2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd4c2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd4c2-107">Die Klasse verwendet, um die Konfiguration der Multi-Mode app für die Kiosk-Konfiguration identifizieren</span><span class="sxs-lookup"><span data-stu-id="bd4c2-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="bd4c2-108">Erbt vom [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd4c2-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd4c2-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd4c2-109">Properties</span></span>
|<span data-ttu-id="bd4c2-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd4c2-110">Property</span></span>|<span data-ttu-id="bd4c2-111">Typ</span><span class="sxs-lookup"><span data-stu-id="bd4c2-111">Type</span></span>|<span data-ttu-id="bd4c2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd4c2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd4c2-113">Apps</span><span class="sxs-lookup"><span data-stu-id="bd4c2-113">apps</span></span>|<span data-ttu-id="bd4c2-114">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bd4c2-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="bd4c2-115">Dies sind die einzige Windows Store-Apps, die über das Startmenü gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="bd4c2-116">Diese Sammlung kann bis zu 128 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-116">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="bd4c2-117">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="bd4c2-117">showTaskBar</span></span>|<span data-ttu-id="bd4c2-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd4c2-118">Boolean</span></span>|<span data-ttu-id="bd4c2-119">Mit dieser Einstellung kann den Administrator an, ob der Taskleiste oder nicht angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-119">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="bd4c2-120">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="bd4c2-120">disallowDesktopApps</span></span>|<span data-ttu-id="bd4c2-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd4c2-121">Boolean</span></span>|<span data-ttu-id="bd4c2-122">Diese Einstellung gibt an, dass desktop-apps zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-122">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="bd4c2-123">Standardmäßig auf "true".</span><span class="sxs-lookup"><span data-stu-id="bd4c2-123">Default to true.</span></span>|
|<span data-ttu-id="bd4c2-124">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="bd4c2-124">startMenuLayoutXml</span></span>|<span data-ttu-id="bd4c2-125">Binär</span><span class="sxs-lookup"><span data-stu-id="bd4c2-125">Binary</span></span>|<span data-ttu-id="bd4c2-126">Ermöglicht Administratoren das Standardlayout Start außer Kraft gesetzt, und verhindert, dass den Benutzer geändert wird.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-126">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="bd4c2-127">Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-127"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="bd4c2-128">XML muss im Binärformat sein.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-128">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd4c2-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bd4c2-129">Relationships</span></span>
<span data-ttu-id="bd4c2-130">Keine</span><span class="sxs-lookup"><span data-stu-id="bd4c2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd4c2-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd4c2-131">JSON Representation</span></span>
<span data-ttu-id="bd4c2-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd4c2-132">Here is a JSON representation of the resource.</span></span>
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
      "appType": "String",
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




