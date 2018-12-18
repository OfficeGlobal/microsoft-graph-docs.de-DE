---
title: Ressourcentyp sharedAppleDeviceUser
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 4e16d691ed6286fb8046c0693292012e1e94a0ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315989"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="41bef-103">Ressourcentyp sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="41bef-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="41bef-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="41bef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41bef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="41bef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41bef-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="41bef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41bef-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="41bef-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="41bef-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="41bef-108">Properties</span></span>
|<span data-ttu-id="41bef-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41bef-109">Property</span></span>|<span data-ttu-id="41bef-110">Typ</span><span class="sxs-lookup"><span data-stu-id="41bef-110">Type</span></span>|<span data-ttu-id="41bef-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41bef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41bef-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41bef-112">userPrincipalName</span></span>|<span data-ttu-id="41bef-113">String</span><span class="sxs-lookup"><span data-stu-id="41bef-113">String</span></span>|<span data-ttu-id="41bef-114">Benutzername</span><span class="sxs-lookup"><span data-stu-id="41bef-114">User name</span></span>|
|<span data-ttu-id="41bef-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="41bef-115">dataToSync</span></span>|<span data-ttu-id="41bef-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="41bef-116">Boolean</span></span>|<span data-ttu-id="41bef-117">Daten synchronisieren</span><span class="sxs-lookup"><span data-stu-id="41bef-117">Data to sync</span></span>|
|<span data-ttu-id="41bef-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="41bef-118">dataQuota</span></span>|<span data-ttu-id="41bef-119">Int64</span><span class="sxs-lookup"><span data-stu-id="41bef-119">Int64</span></span>|<span data-ttu-id="41bef-120">Datenträgerkontingent</span><span class="sxs-lookup"><span data-stu-id="41bef-120">Data quota</span></span>|
|<span data-ttu-id="41bef-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="41bef-121">dataUsed</span></span>|<span data-ttu-id="41bef-122">Int64</span><span class="sxs-lookup"><span data-stu-id="41bef-122">Int64</span></span>|<span data-ttu-id="41bef-123">Datenträgerkontingent</span><span class="sxs-lookup"><span data-stu-id="41bef-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="41bef-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="41bef-124">Relationships</span></span>
<span data-ttu-id="41bef-125">Keine</span><span class="sxs-lookup"><span data-stu-id="41bef-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="41bef-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="41bef-126">JSON Representation</span></span>
<span data-ttu-id="41bef-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="41bef-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```





