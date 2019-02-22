---
title: sharedAppleDeviceUser-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f737432597d4528d1a682cd15552230af0ae83e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156504"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="725ef-103">sharedAppleDeviceUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="725ef-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="725ef-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="725ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="725ef-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="725ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="725ef-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="725ef-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="725ef-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="725ef-107">Properties</span></span>
|<span data-ttu-id="725ef-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="725ef-108">Property</span></span>|<span data-ttu-id="725ef-109">Typ</span><span class="sxs-lookup"><span data-stu-id="725ef-109">Type</span></span>|<span data-ttu-id="725ef-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="725ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="725ef-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="725ef-111">userPrincipalName</span></span>|<span data-ttu-id="725ef-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="725ef-112">String</span></span>|<span data-ttu-id="725ef-113">Benutzername</span><span class="sxs-lookup"><span data-stu-id="725ef-113">User name</span></span>|
|<span data-ttu-id="725ef-114">dataToSync</span><span class="sxs-lookup"><span data-stu-id="725ef-114">dataToSync</span></span>|<span data-ttu-id="725ef-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="725ef-115">Boolean</span></span>|<span data-ttu-id="725ef-116">Zu synchronisierende Daten</span><span class="sxs-lookup"><span data-stu-id="725ef-116">Data to sync</span></span>|
|<span data-ttu-id="725ef-117">dataQuota</span><span class="sxs-lookup"><span data-stu-id="725ef-117">dataQuota</span></span>|<span data-ttu-id="725ef-118">Int64</span><span class="sxs-lookup"><span data-stu-id="725ef-118">Int64</span></span>|<span data-ttu-id="725ef-119">Datenkontingent</span><span class="sxs-lookup"><span data-stu-id="725ef-119">Data quota</span></span>|
|<span data-ttu-id="725ef-120">dataUsed</span><span class="sxs-lookup"><span data-stu-id="725ef-120">dataUsed</span></span>|<span data-ttu-id="725ef-121">Int64</span><span class="sxs-lookup"><span data-stu-id="725ef-121">Int64</span></span>|<span data-ttu-id="725ef-122">Datenkontingent</span><span class="sxs-lookup"><span data-stu-id="725ef-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="725ef-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="725ef-123">Relationships</span></span>
<span data-ttu-id="725ef-124">Keine</span><span class="sxs-lookup"><span data-stu-id="725ef-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="725ef-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="725ef-125">JSON Representation</span></span>
<span data-ttu-id="725ef-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="725ef-126">Here is a JSON representation of the resource.</span></span>
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




