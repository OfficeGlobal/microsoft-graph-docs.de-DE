---
title: Ressourcentyp windowsKioskActiveDirectoryGroup
description: Die Klasse, die zur Identifizierung einer Azure-Directory-Gruppe für die Kiosk-Konfiguration
author: tfitzmac
ms.openlocfilehash: 618b93182d17d485a35d2567f45c218c6117658f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331774"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="bca50-103">Ressourcentyp windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="bca50-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="bca50-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bca50-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bca50-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bca50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bca50-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bca50-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bca50-107">Die Klasse, die zur Identifizierung einer Azure-Directory-Gruppe für die Kiosk-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="bca50-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>

<span data-ttu-id="bca50-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="bca50-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bca50-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bca50-109">Properties</span></span>
|<span data-ttu-id="bca50-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bca50-110">Property</span></span>|<span data-ttu-id="bca50-111">Typ</span><span class="sxs-lookup"><span data-stu-id="bca50-111">Type</span></span>|<span data-ttu-id="bca50-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bca50-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca50-113">groupName</span><span class="sxs-lookup"><span data-stu-id="bca50-113">groupName</span></span>|<span data-ttu-id="bca50-114">String</span><span class="sxs-lookup"><span data-stu-id="bca50-114">String</span></span>|<span data-ttu-id="bca50-115">Der Name des AD-Gruppe ein, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="bca50-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="bca50-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bca50-116">Relationships</span></span>
<span data-ttu-id="bca50-117">Keine</span><span class="sxs-lookup"><span data-stu-id="bca50-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bca50-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bca50-118">JSON Representation</span></span>
<span data-ttu-id="bca50-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bca50-119">Here is a JSON representation of the resource.</span></span>
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





