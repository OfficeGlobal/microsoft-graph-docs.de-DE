---
title: Ressourcentyp sharedAppleDeviceUser
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5ee74080b95328cf55813dc628ee7a517dff08e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806853"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="b3090-103">Ressourcentyp sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="b3090-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="b3090-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3090-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3090-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3090-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3090-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b3090-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3090-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b3090-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b3090-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b3090-108">Properties</span></span>
|<span data-ttu-id="b3090-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3090-109">Property</span></span>|<span data-ttu-id="b3090-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b3090-110">Type</span></span>|<span data-ttu-id="b3090-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3090-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3090-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b3090-112">userPrincipalName</span></span>|<span data-ttu-id="b3090-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3090-113">String</span></span>|<span data-ttu-id="b3090-114">Benutzername</span><span class="sxs-lookup"><span data-stu-id="b3090-114">User name</span></span>|
|<span data-ttu-id="b3090-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="b3090-115">dataToSync</span></span>|<span data-ttu-id="b3090-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b3090-116">Boolean</span></span>|<span data-ttu-id="b3090-117">Daten synchronisieren</span><span class="sxs-lookup"><span data-stu-id="b3090-117">Data to sync</span></span>|
|<span data-ttu-id="b3090-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="b3090-118">dataQuota</span></span>|<span data-ttu-id="b3090-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b3090-119">Int64</span></span>|<span data-ttu-id="b3090-120">Datenträgerkontingent</span><span class="sxs-lookup"><span data-stu-id="b3090-120">Data quota</span></span>|
|<span data-ttu-id="b3090-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="b3090-121">dataUsed</span></span>|<span data-ttu-id="b3090-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b3090-122">Int64</span></span>|<span data-ttu-id="b3090-123">Datenträgerkontingent</span><span class="sxs-lookup"><span data-stu-id="b3090-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3090-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b3090-124">Relationships</span></span>
<span data-ttu-id="b3090-125">Keine</span><span class="sxs-lookup"><span data-stu-id="b3090-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3090-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b3090-126">JSON Representation</span></span>
<span data-ttu-id="b3090-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b3090-127">Here is a JSON representation of the resource.</span></span>
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





