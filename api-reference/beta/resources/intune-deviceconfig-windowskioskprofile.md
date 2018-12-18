---
title: Ressourcentyp windowsKioskProfile
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: ce57b18e86f40a46053a5e0a0f41652763a6d055
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345353"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="3736f-103">Ressourcentyp windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="3736f-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="3736f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3736f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3736f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3736f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3736f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3736f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3736f-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3736f-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3736f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3736f-108">Properties</span></span>
|<span data-ttu-id="3736f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3736f-109">Property</span></span>|<span data-ttu-id="3736f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3736f-110">Type</span></span>|<span data-ttu-id="3736f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3736f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3736f-112">ID</span><span class="sxs-lookup"><span data-stu-id="3736f-112">profileId</span></span>|<span data-ttu-id="3736f-113">String</span><span class="sxs-lookup"><span data-stu-id="3736f-113">String</span></span>|<span data-ttu-id="3736f-114">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3736f-114">Key of the entity.</span></span>|
|<span data-ttu-id="3736f-115">Profilname</span><span class="sxs-lookup"><span data-stu-id="3736f-115">profileName</span></span>|<span data-ttu-id="3736f-116">String</span><span class="sxs-lookup"><span data-stu-id="3736f-116">String</span></span>|<span data-ttu-id="3736f-117">Dies ist ein Anzeigename zur Identifizierung einer Gruppe von Anwendungen, das Layout von diese apps auf das Startmenü und die Benutzer, die diese Konfiguration Kiosk zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="3736f-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="3736f-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="3736f-118">appConfiguration</span></span>|[<span data-ttu-id="3736f-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3736f-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="3736f-120">Die App-Konfiguration, die für diese Konfiguration Kiosk verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3736f-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="3736f-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="3736f-121">userAccountsConfiguration</span></span>|<span data-ttu-id="3736f-122">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3736f-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="3736f-123">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt werden.</span><span class="sxs-lookup"><span data-stu-id="3736f-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="3736f-124">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="3736f-124">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3736f-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3736f-125">Relationships</span></span>
<span data-ttu-id="3736f-126">Keine</span><span class="sxs-lookup"><span data-stu-id="3736f-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3736f-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3736f-127">JSON Representation</span></span>
<span data-ttu-id="3736f-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3736f-128">Here is a JSON representation of the resource.</span></span>
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





