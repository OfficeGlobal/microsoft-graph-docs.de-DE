---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66c4fc3c724eecf3a05dae24cb3f6a52de82d059
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255850"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="50a9f-103">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="50a9f-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="50a9f-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="50a9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50a9f-105">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="50a9f-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="50a9f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50a9f-106">Properties</span></span>
|<span data-ttu-id="50a9f-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50a9f-107">Property</span></span>|<span data-ttu-id="50a9f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="50a9f-108">Type</span></span>|<span data-ttu-id="50a9f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50a9f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a9f-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="50a9f-110">encryptionKey</span></span>|<span data-ttu-id="50a9f-111">Binär</span><span class="sxs-lookup"><span data-stu-id="50a9f-111">Binary</span></span>|<span data-ttu-id="50a9f-112">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="50a9f-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="50a9f-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="50a9f-113">initializationVector</span></span>|<span data-ttu-id="50a9f-114">Binär</span><span class="sxs-lookup"><span data-stu-id="50a9f-114">Binary</span></span>|<span data-ttu-id="50a9f-115">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="50a9f-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="50a9f-116">mac</span><span class="sxs-lookup"><span data-stu-id="50a9f-116">mac</span></span>|<span data-ttu-id="50a9f-117">Binär</span><span class="sxs-lookup"><span data-stu-id="50a9f-117">Binary</span></span>|<span data-ttu-id="50a9f-118">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="50a9f-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="50a9f-119">macKey</span><span class="sxs-lookup"><span data-stu-id="50a9f-119">macKey</span></span>|<span data-ttu-id="50a9f-120">Binär</span><span class="sxs-lookup"><span data-stu-id="50a9f-120">Binary</span></span>|<span data-ttu-id="50a9f-121">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="50a9f-121">The key used to get mac.</span></span>|
|<span data-ttu-id="50a9f-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="50a9f-122">profileIdentifier</span></span>|<span data-ttu-id="50a9f-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50a9f-123">String</span></span>|<span data-ttu-id="50a9f-124">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="50a9f-124">The the profile identifier.</span></span>|
|<span data-ttu-id="50a9f-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="50a9f-125">fileDigest</span></span>|<span data-ttu-id="50a9f-126">Binary</span><span class="sxs-lookup"><span data-stu-id="50a9f-126">Binary</span></span>|<span data-ttu-id="50a9f-127">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="50a9f-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="50a9f-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="50a9f-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="50a9f-129">String</span><span class="sxs-lookup"><span data-stu-id="50a9f-129">String</span></span>|<span data-ttu-id="50a9f-130">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="50a9f-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50a9f-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="50a9f-131">Relationships</span></span>
<span data-ttu-id="50a9f-132">Keine</span><span class="sxs-lookup"><span data-stu-id="50a9f-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50a9f-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50a9f-133">JSON Representation</span></span>
<span data-ttu-id="50a9f-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50a9f-134">Here is a JSON representation of the resource.</span></span>
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



