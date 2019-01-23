---
title: Ressourcentyp windowsKioskProfile
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55d8c23d3bfae2baf9d632c33390b8aafb5e7ef8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420248"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="4011e-103">Ressourcentyp windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="4011e-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="4011e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4011e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4011e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4011e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4011e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4011e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4011e-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4011e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4011e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4011e-108">Properties</span></span>
|<span data-ttu-id="4011e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4011e-109">Property</span></span>|<span data-ttu-id="4011e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4011e-110">Type</span></span>|<span data-ttu-id="4011e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4011e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4011e-112">ID</span><span class="sxs-lookup"><span data-stu-id="4011e-112">profileId</span></span>|<span data-ttu-id="4011e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4011e-113">String</span></span>|<span data-ttu-id="4011e-114">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4011e-114">Key of the entity.</span></span>|
|<span data-ttu-id="4011e-115">Profilname</span><span class="sxs-lookup"><span data-stu-id="4011e-115">profileName</span></span>|<span data-ttu-id="4011e-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4011e-116">String</span></span>|<span data-ttu-id="4011e-117">Dies ist ein Anzeigename zur Identifizierung einer Gruppe von Anwendungen, das Layout von diese apps auf das Startmenü und die Benutzer, die diese Konfiguration Kiosk zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="4011e-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="4011e-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="4011e-118">appConfiguration</span></span>|[<span data-ttu-id="4011e-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4011e-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="4011e-120">Die App-Konfiguration, die für diese Konfiguration Kiosk verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4011e-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="4011e-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4011e-121">userAccountsConfiguration</span></span>|<span data-ttu-id="4011e-122">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4011e-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="4011e-123">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt werden.</span><span class="sxs-lookup"><span data-stu-id="4011e-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="4011e-124">Diese Sammlung kann maximal 100 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4011e-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4011e-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4011e-125">Relationships</span></span>
<span data-ttu-id="4011e-126">Keine</span><span class="sxs-lookup"><span data-stu-id="4011e-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4011e-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4011e-127">JSON Representation</span></span>
<span data-ttu-id="4011e-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4011e-128">Here is a JSON representation of the resource.</span></span>
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




