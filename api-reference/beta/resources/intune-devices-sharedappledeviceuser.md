---
title: Ressourcentyp sharedAppleDeviceUser
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6106daff0b7c4af023c8bfbb8352b52efc674928
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987706"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="f6c34-103">Ressourcentyp sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="f6c34-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="f6c34-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6c34-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6c34-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6c34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6c34-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f6c34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6c34-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f6c34-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f6c34-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6c34-108">Properties</span></span>
|<span data-ttu-id="f6c34-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6c34-109">Property</span></span>|<span data-ttu-id="f6c34-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f6c34-110">Type</span></span>|<span data-ttu-id="f6c34-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6c34-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6c34-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6c34-112">userPrincipalName</span></span>|<span data-ttu-id="f6c34-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6c34-113">String</span></span>|<span data-ttu-id="f6c34-114">Benutzername</span><span class="sxs-lookup"><span data-stu-id="f6c34-114">User name</span></span>|
|<span data-ttu-id="f6c34-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="f6c34-115">dataToSync</span></span>|<span data-ttu-id="f6c34-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f6c34-116">Boolean</span></span>|<span data-ttu-id="f6c34-117">Daten synchronisieren</span><span class="sxs-lookup"><span data-stu-id="f6c34-117">Data to sync</span></span>|
|<span data-ttu-id="f6c34-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="f6c34-118">dataQuota</span></span>|<span data-ttu-id="f6c34-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f6c34-119">Int64</span></span>|<span data-ttu-id="f6c34-120">Datenträgerkontingent</span><span class="sxs-lookup"><span data-stu-id="f6c34-120">Data quota</span></span>|
|<span data-ttu-id="f6c34-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="f6c34-121">dataUsed</span></span>|<span data-ttu-id="f6c34-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f6c34-122">Int64</span></span>|<span data-ttu-id="f6c34-123">Datenträgerkontingent</span><span class="sxs-lookup"><span data-stu-id="f6c34-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6c34-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f6c34-124">Relationships</span></span>
<span data-ttu-id="f6c34-125">Keine</span><span class="sxs-lookup"><span data-stu-id="f6c34-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6c34-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6c34-126">JSON Representation</span></span>
<span data-ttu-id="f6c34-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6c34-127">Here is a JSON representation of the resource.</span></span>
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





