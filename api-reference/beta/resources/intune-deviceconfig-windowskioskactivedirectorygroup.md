---
title: Ressourcentyp windowsKioskActiveDirectoryGroup
description: Die Klasse, die zur Identifizierung einer Azure-Directory-Gruppe für die Kiosk-Konfiguration
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 88b151b856809247cfa6e5e211cc45c6f33c4c53
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415712"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="ec3d1-103">Ressourcentyp windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="ec3d1-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="ec3d1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ec3d1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ec3d1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec3d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec3d1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec3d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec3d1-107">Die Klasse, die zur Identifizierung einer Azure-Directory-Gruppe für die Kiosk-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="ec3d1-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="ec3d1-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="ec3d1-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec3d1-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ec3d1-109">Properties</span></span>
|<span data-ttu-id="ec3d1-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec3d1-110">Property</span></span>|<span data-ttu-id="ec3d1-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ec3d1-111">Type</span></span>|<span data-ttu-id="ec3d1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec3d1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec3d1-113">groupName</span><span class="sxs-lookup"><span data-stu-id="ec3d1-113">groupName</span></span>|<span data-ttu-id="ec3d1-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec3d1-114">String</span></span>|<span data-ttu-id="ec3d1-115">Der Name des AD-Gruppe ein, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="ec3d1-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec3d1-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ec3d1-116">Relationships</span></span>
<span data-ttu-id="ec3d1-117">Keine</span><span class="sxs-lookup"><span data-stu-id="ec3d1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec3d1-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ec3d1-118">JSON Representation</span></span>
<span data-ttu-id="ec3d1-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ec3d1-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```




