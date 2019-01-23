---
title: Ressourcentyp sharedAppleDeviceUser
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 46e0993c69a8ae34a54a654959d8d67a1b7f4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394432"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="042cd-103">Ressourcentyp sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="042cd-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="042cd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="042cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="042cd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="042cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="042cd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="042cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="042cd-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="042cd-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="042cd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="042cd-108">Properties</span></span>
|<span data-ttu-id="042cd-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="042cd-109">Property</span></span>|<span data-ttu-id="042cd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="042cd-110">Type</span></span>|<span data-ttu-id="042cd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="042cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="042cd-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="042cd-112">userPrincipalName</span></span>|<span data-ttu-id="042cd-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="042cd-113">String</span></span>|<span data-ttu-id="042cd-114">Benutzername</span><span class="sxs-lookup"><span data-stu-id="042cd-114">User name</span></span>|
|<span data-ttu-id="042cd-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="042cd-115">dataToSync</span></span>|<span data-ttu-id="042cd-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="042cd-116">Boolean</span></span>|<span data-ttu-id="042cd-117">Daten synchronisieren</span><span class="sxs-lookup"><span data-stu-id="042cd-117">Data to sync</span></span>|
|<span data-ttu-id="042cd-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="042cd-118">dataQuota</span></span>|<span data-ttu-id="042cd-119">Int64</span><span class="sxs-lookup"><span data-stu-id="042cd-119">Int64</span></span>|<span data-ttu-id="042cd-120">Datenträgerkontingent</span><span class="sxs-lookup"><span data-stu-id="042cd-120">Data quota</span></span>|
|<span data-ttu-id="042cd-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="042cd-121">dataUsed</span></span>|<span data-ttu-id="042cd-122">Int64</span><span class="sxs-lookup"><span data-stu-id="042cd-122">Int64</span></span>|<span data-ttu-id="042cd-123">Datenträgerkontingent</span><span class="sxs-lookup"><span data-stu-id="042cd-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="042cd-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="042cd-124">Relationships</span></span>
<span data-ttu-id="042cd-125">Keine</span><span class="sxs-lookup"><span data-stu-id="042cd-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="042cd-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="042cd-126">JSON Representation</span></span>
<span data-ttu-id="042cd-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="042cd-127">Here is a JSON representation of the resource.</span></span>
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




