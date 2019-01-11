---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbc52cfd4e14b2010dd133e4fa08e61a30fb63df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814112"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="169b6-103">vppLicensingType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="169b6-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="169b6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="169b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="169b6-105">Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.</span><span class="sxs-lookup"><span data-stu-id="169b6-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="169b6-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="169b6-106">Properties</span></span>
|<span data-ttu-id="169b6-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="169b6-107">Property</span></span>|<span data-ttu-id="169b6-108">Typ</span><span class="sxs-lookup"><span data-stu-id="169b6-108">Type</span></span>|<span data-ttu-id="169b6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="169b6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="169b6-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="169b6-110">supportsUserLicensing</span></span>|<span data-ttu-id="169b6-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="169b6-111">Boolean</span></span>|<span data-ttu-id="169b6-112">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="169b6-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="169b6-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="169b6-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="169b6-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="169b6-114">Boolean</span></span>|<span data-ttu-id="169b6-115">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="169b6-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="169b6-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="169b6-116">Relationships</span></span>
<span data-ttu-id="169b6-117">Keine</span><span class="sxs-lookup"><span data-stu-id="169b6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="169b6-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="169b6-118">JSON Representation</span></span>
<span data-ttu-id="169b6-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="169b6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



