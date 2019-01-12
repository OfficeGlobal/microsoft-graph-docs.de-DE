---
title: Ressourcentyp windowsKioskProfile
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fc462bdf6548f0f281082ba1cb228796899896d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977052"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="2be99-103">Ressourcentyp windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="2be99-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="2be99-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2be99-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2be99-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2be99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2be99-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2be99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2be99-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2be99-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2be99-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2be99-108">Properties</span></span>
|<span data-ttu-id="2be99-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2be99-109">Property</span></span>|<span data-ttu-id="2be99-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2be99-110">Type</span></span>|<span data-ttu-id="2be99-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2be99-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2be99-112">ID</span><span class="sxs-lookup"><span data-stu-id="2be99-112">profileId</span></span>|<span data-ttu-id="2be99-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2be99-113">String</span></span>|<span data-ttu-id="2be99-114">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2be99-114">Key of the entity.</span></span>|
|<span data-ttu-id="2be99-115">Profilname</span><span class="sxs-lookup"><span data-stu-id="2be99-115">profileName</span></span>|<span data-ttu-id="2be99-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2be99-116">String</span></span>|<span data-ttu-id="2be99-117">Dies ist ein Anzeigename zur Identifizierung einer Gruppe von Anwendungen, das Layout von diese apps auf das Startmenü und die Benutzer, die diese Konfiguration Kiosk zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="2be99-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="2be99-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="2be99-118">appConfiguration</span></span>|[<span data-ttu-id="2be99-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2be99-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="2be99-120">Die App-Konfiguration, die für diese Konfiguration Kiosk verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="2be99-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="2be99-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2be99-121">userAccountsConfiguration</span></span>|<span data-ttu-id="2be99-122">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="2be99-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="2be99-123">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt werden.</span><span class="sxs-lookup"><span data-stu-id="2be99-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="2be99-124">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="2be99-124">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2be99-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2be99-125">Relationships</span></span>
<span data-ttu-id="2be99-126">Keine</span><span class="sxs-lookup"><span data-stu-id="2be99-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2be99-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2be99-127">JSON Representation</span></span>
<span data-ttu-id="2be99-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2be99-128">Here is a JSON representation of the resource.</span></span>
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





