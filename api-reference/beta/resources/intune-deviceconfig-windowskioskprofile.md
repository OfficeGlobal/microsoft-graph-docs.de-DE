---
title: windowsKioskProfile-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1c7107982a33452cd9dd00829cba08f108c6394
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164750"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="83791-103">windowsKioskProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="83791-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="83791-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83791-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83791-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="83791-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83791-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="83791-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="83791-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83791-107">Properties</span></span>
|<span data-ttu-id="83791-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83791-108">Property</span></span>|<span data-ttu-id="83791-109">Typ</span><span class="sxs-lookup"><span data-stu-id="83791-109">Type</span></span>|<span data-ttu-id="83791-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83791-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83791-111">profileId</span><span class="sxs-lookup"><span data-stu-id="83791-111">profileId</span></span>|<span data-ttu-id="83791-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83791-112">String</span></span>|<span data-ttu-id="83791-113">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="83791-113">Key of the entity.</span></span>|
|<span data-ttu-id="83791-114">Profilname</span><span class="sxs-lookup"><span data-stu-id="83791-114">profileName</span></span>|<span data-ttu-id="83791-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83791-115">String</span></span>|<span data-ttu-id="83791-116">Dies ist ein Anzeigename, der verwendet wird, um eine Gruppe von Anwendungen, das Layout dieser apps im Startmenü und die Benutzer zu identifizieren, denen diese Kiosk Konfiguration zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="83791-116">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="83791-117">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="83791-117">appConfiguration</span></span>|[<span data-ttu-id="83791-118">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="83791-118">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="83791-119">Die APP-Konfiguration, die für diese Kiosk Konfiguration verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="83791-119">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="83791-120">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="83791-120">userAccountsConfiguration</span></span>|<span data-ttu-id="83791-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="83791-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="83791-122">Die Benutzerkonten, die für diese Kiosk Konfiguration gesperrt werden.</span><span class="sxs-lookup"><span data-stu-id="83791-122">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="83791-123">Diese Auflistung kann maximal 100 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="83791-123">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83791-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="83791-124">Relationships</span></span>
<span data-ttu-id="83791-125">Keine</span><span class="sxs-lookup"><span data-stu-id="83791-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83791-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83791-126">JSON Representation</span></span>
<span data-ttu-id="83791-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83791-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
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
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```




