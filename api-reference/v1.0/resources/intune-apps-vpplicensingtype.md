---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
ms.openlocfilehash: 4e02cc4ee100fe9fa6be0eb116cff18e343fd8ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016737"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="0a20f-103">vppLicensingType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0a20f-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="0a20f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0a20f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a20f-105">Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.</span><span class="sxs-lookup"><span data-stu-id="0a20f-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="0a20f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a20f-106">Properties</span></span>
|<span data-ttu-id="0a20f-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a20f-107">Property</span></span>|<span data-ttu-id="0a20f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0a20f-108">Type</span></span>|<span data-ttu-id="0a20f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a20f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a20f-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="0a20f-110">supportsUserLicensing</span></span>|<span data-ttu-id="0a20f-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0a20f-111">Boolean</span></span>|<span data-ttu-id="0a20f-112">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a20f-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="0a20f-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="0a20f-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="0a20f-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0a20f-114">Boolean</span></span>|<span data-ttu-id="0a20f-115">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a20f-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a20f-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0a20f-116">Relationships</span></span>
<span data-ttu-id="0a20f-117">Keine</span><span class="sxs-lookup"><span data-stu-id="0a20f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a20f-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0a20f-118">JSON Representation</span></span>
<span data-ttu-id="0a20f-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0a20f-119">Here is a JSON representation of the resource.</span></span>
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



