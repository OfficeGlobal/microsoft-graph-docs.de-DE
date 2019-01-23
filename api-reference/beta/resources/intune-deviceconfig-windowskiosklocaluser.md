---
title: Ressourcentyp windowsKioskLocalUser
description: Die Klasse verwendet, um ein lokales Konto für die Konfiguration Kiosk identifizieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b808cdb6cb8bb8540a553104d2c00108341a3e14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392668"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="a4dcc-103">Ressourcentyp windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="a4dcc-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="a4dcc-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a4dcc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a4dcc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4dcc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4dcc-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a4dcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4dcc-107">Die Klasse verwendet, um ein lokales Konto für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="a4dcc-107">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="a4dcc-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="a4dcc-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a4dcc-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a4dcc-109">Properties</span></span>
|<span data-ttu-id="a4dcc-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a4dcc-110">Property</span></span>|<span data-ttu-id="a4dcc-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a4dcc-111">Type</span></span>|<span data-ttu-id="a4dcc-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4dcc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4dcc-113">userName</span><span class="sxs-lookup"><span data-stu-id="a4dcc-113">userName</span></span>|<span data-ttu-id="a4dcc-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4dcc-114">String</span></span>|<span data-ttu-id="a4dcc-115">Der lokale Benutzer, der mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="a4dcc-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4dcc-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a4dcc-116">Relationships</span></span>
<span data-ttu-id="a4dcc-117">Keine</span><span class="sxs-lookup"><span data-stu-id="a4dcc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4dcc-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a4dcc-118">JSON Representation</span></span>
<span data-ttu-id="a4dcc-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a4dcc-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```




