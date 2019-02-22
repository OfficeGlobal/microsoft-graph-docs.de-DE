---
title: appLogCollectionDownloadDetails-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3449e1f1a2b8651cea407690019d458d5ac24fa9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147754"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="8c5d7-103">appLogCollectionDownloadDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8c5d7-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="8c5d7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c5d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c5d7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8c5d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c5d7-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8c5d7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8c5d7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8c5d7-107">Properties</span></span>
|<span data-ttu-id="8c5d7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c5d7-108">Property</span></span>|<span data-ttu-id="8c5d7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8c5d7-109">Type</span></span>|<span data-ttu-id="8c5d7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c5d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c5d7-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="8c5d7-111">downloadUrl</span></span>|<span data-ttu-id="8c5d7-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8c5d7-112">String</span></span>|<span data-ttu-id="8c5d7-113">Download der SAS-URL für completed AppLogUploadRequest</span><span class="sxs-lookup"><span data-stu-id="8c5d7-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="8c5d7-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="8c5d7-114">decryptionKey</span></span>|<span data-ttu-id="8c5d7-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8c5d7-115">String</span></span>|<span data-ttu-id="8c5d7-116">DecryptionKey als Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8c5d7-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="8c5d7-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8c5d7-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="8c5d7-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8c5d7-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="8c5d7-119">DecryptionAlgorithm für Inhalt.</span><span class="sxs-lookup"><span data-stu-id="8c5d7-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="8c5d7-120">Mögliche Werte sind: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="8c5d7-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c5d7-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8c5d7-121">Relationships</span></span>
<span data-ttu-id="8c5d7-122">Keine</span><span class="sxs-lookup"><span data-stu-id="8c5d7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c5d7-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8c5d7-123">JSON Representation</span></span>
<span data-ttu-id="8c5d7-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8c5d7-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```




