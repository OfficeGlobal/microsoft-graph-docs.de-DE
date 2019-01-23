---
title: Ressourcentyp appLogCollectionDownloadDetails
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6946b3cd1aa60c4025859bd8d41d2dc4775bf39d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429920"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="039f1-103">Ressourcentyp appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="039f1-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="039f1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="039f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="039f1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="039f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="039f1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="039f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="039f1-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="039f1-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="039f1-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="039f1-108">Properties</span></span>
|<span data-ttu-id="039f1-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="039f1-109">Property</span></span>|<span data-ttu-id="039f1-110">Typ</span><span class="sxs-lookup"><span data-stu-id="039f1-110">Type</span></span>|<span data-ttu-id="039f1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="039f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="039f1-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="039f1-112">downloadUrl</span></span>|<span data-ttu-id="039f1-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039f1-113">String</span></span>|<span data-ttu-id="039f1-114">SAS-Url für abgeschlossene AppLogUploadRequest herunterladen</span><span class="sxs-lookup"><span data-stu-id="039f1-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="039f1-115">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="039f1-115">decryptionKey</span></span>|<span data-ttu-id="039f1-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039f1-116">String</span></span>|<span data-ttu-id="039f1-117">DecryptionKey als Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039f1-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="039f1-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="039f1-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="039f1-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="039f1-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="039f1-120">DecryptionAlgorithm für Inhalte.</span><span class="sxs-lookup"><span data-stu-id="039f1-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="039f1-121">Mögliche Werte sind: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="039f1-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="039f1-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="039f1-122">Relationships</span></span>
<span data-ttu-id="039f1-123">Keine</span><span class="sxs-lookup"><span data-stu-id="039f1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="039f1-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="039f1-124">JSON Representation</span></span>
<span data-ttu-id="039f1-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="039f1-125">Here is a JSON representation of the resource.</span></span>
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




