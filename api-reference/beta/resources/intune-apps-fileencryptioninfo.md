---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 060f8eac1bfff3f0d2e18d52428deb884da4a759
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168572"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="9acf8-103">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9acf8-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="9acf8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9acf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9acf8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9acf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9acf8-106">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="9acf8-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="9acf8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9acf8-107">Properties</span></span>
|<span data-ttu-id="9acf8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9acf8-108">Property</span></span>|<span data-ttu-id="9acf8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9acf8-109">Type</span></span>|<span data-ttu-id="9acf8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9acf8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9acf8-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="9acf8-111">encryptionKey</span></span>|<span data-ttu-id="9acf8-112">Binär</span><span class="sxs-lookup"><span data-stu-id="9acf8-112">Binary</span></span>|<span data-ttu-id="9acf8-113">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="9acf8-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="9acf8-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="9acf8-114">initializationVector</span></span>|<span data-ttu-id="9acf8-115">Binär</span><span class="sxs-lookup"><span data-stu-id="9acf8-115">Binary</span></span>|<span data-ttu-id="9acf8-116">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="9acf8-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="9acf8-117">mac</span><span class="sxs-lookup"><span data-stu-id="9acf8-117">mac</span></span>|<span data-ttu-id="9acf8-118">Binär</span><span class="sxs-lookup"><span data-stu-id="9acf8-118">Binary</span></span>|<span data-ttu-id="9acf8-119">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="9acf8-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="9acf8-120">macKey</span><span class="sxs-lookup"><span data-stu-id="9acf8-120">macKey</span></span>|<span data-ttu-id="9acf8-121">Binär</span><span class="sxs-lookup"><span data-stu-id="9acf8-121">Binary</span></span>|<span data-ttu-id="9acf8-122">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="9acf8-122">The key used to get mac.</span></span>|
|<span data-ttu-id="9acf8-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="9acf8-123">profileIdentifier</span></span>|<span data-ttu-id="9acf8-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9acf8-124">String</span></span>|<span data-ttu-id="9acf8-125">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="9acf8-125">The the profile identifier.</span></span>|
|<span data-ttu-id="9acf8-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="9acf8-126">fileDigest</span></span>|<span data-ttu-id="9acf8-127">Binary</span><span class="sxs-lookup"><span data-stu-id="9acf8-127">Binary</span></span>|<span data-ttu-id="9acf8-128">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="9acf8-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="9acf8-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="9acf8-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="9acf8-130">String</span><span class="sxs-lookup"><span data-stu-id="9acf8-130">String</span></span>|<span data-ttu-id="9acf8-131">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="9acf8-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9acf8-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9acf8-132">Relationships</span></span>
<span data-ttu-id="9acf8-133">Keine</span><span class="sxs-lookup"><span data-stu-id="9acf8-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9acf8-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9acf8-134">JSON Representation</span></span>
<span data-ttu-id="9acf8-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9acf8-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```




