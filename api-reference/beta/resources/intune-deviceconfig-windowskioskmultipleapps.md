---
title: windowsKioskMultipleApps-Ressourcentyp
description: Die Klasse, die zum Identifizieren der multiMode-App-Konfiguration für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c657300cf3ca00482b85b7983f28b4df3135c97d
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570843"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="1179e-103">windowsKioskMultipleApps-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1179e-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="1179e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1179e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1179e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1179e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1179e-106">Die Klasse, die zum Identifizieren der multiMode-App-Konfiguration für die Kiosk Konfiguration verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1179e-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="1179e-107">Erbt von [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1179e-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1179e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1179e-108">Properties</span></span>
|<span data-ttu-id="1179e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1179e-109">Property</span></span>|<span data-ttu-id="1179e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1179e-110">Type</span></span>|<span data-ttu-id="1179e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1179e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1179e-112">apps</span><span class="sxs-lookup"><span data-stu-id="1179e-112">apps</span></span>|<span data-ttu-id="1179e-113">[zum](../resources/intune-deviceconfig-windowskioskappbase.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="1179e-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="1179e-114">Dies sind die einzigen Windows Store-Apps, die über das Startmenü zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="1179e-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="1179e-115">Diese Auflistung kann maximal 128 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="1179e-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="1179e-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="1179e-116">showTaskBar</span></span>|<span data-ttu-id="1179e-117">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1179e-117">Boolean</span></span>|<span data-ttu-id="1179e-118">Mit dieser Einstellung kann der Administrator angeben, ob die Vorgangsleiste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="1179e-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="1179e-119">allowAccessToDownloadsFolder</span><span class="sxs-lookup"><span data-stu-id="1179e-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="1179e-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1179e-120">Boolean</span></span>|<span data-ttu-id="1179e-121">Diese Einstellung ermöglicht den Zugriff auf den Ordner Downloads im Datei-Explorer.</span><span class="sxs-lookup"><span data-stu-id="1179e-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="1179e-122">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="1179e-122">disallowDesktopApps</span></span>|<span data-ttu-id="1179e-123">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1179e-123">Boolean</span></span>|<span data-ttu-id="1179e-124">Diese Einstellung gibt an, dass Desktop-Apps zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="1179e-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="1179e-125">Standardwert true.</span><span class="sxs-lookup"><span data-stu-id="1179e-125">Default to true.</span></span>|
|<span data-ttu-id="1179e-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="1179e-126">startMenuLayoutXml</span></span>|<span data-ttu-id="1179e-127">Binär</span><span class="sxs-lookup"><span data-stu-id="1179e-127">Binary</span></span>|<span data-ttu-id="1179e-128">Ermöglicht Administratoren das außer Kraft setzen des Standard Start Layouts und hindert den Benutzer daran, es zu ändern.</span><span class="sxs-lookup"><span data-stu-id="1179e-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="1179e-129">Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert.</span><span class="sxs-lookup"><span data-stu-id="1179e-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="1179e-130">XML muss im Binärformat vorliegen.</span><span class="sxs-lookup"><span data-stu-id="1179e-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1179e-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1179e-131">Relationships</span></span>
<span data-ttu-id="1179e-132">Keine</span><span class="sxs-lookup"><span data-stu-id="1179e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1179e-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1179e-133">JSON Representation</span></span>
<span data-ttu-id="1179e-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1179e-134">Here is a JSON representation of the resource.</span></span>
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
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```




