---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 074bf24638bf0ba7d613399e1b8894de7f30dfbb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410896"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="d5295-103">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d5295-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="d5295-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d5295-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5295-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5295-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5295-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d5295-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5295-107">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="d5295-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="d5295-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d5295-108">Properties</span></span>
|<span data-ttu-id="d5295-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5295-109">Property</span></span>|<span data-ttu-id="d5295-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d5295-110">Type</span></span>|<span data-ttu-id="d5295-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5295-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5295-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="d5295-112">encryptionKey</span></span>|<span data-ttu-id="d5295-113">Binary</span><span class="sxs-lookup"><span data-stu-id="d5295-113">Binary</span></span>|<span data-ttu-id="d5295-114">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d5295-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="d5295-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="d5295-115">initializationVector</span></span>|<span data-ttu-id="d5295-116">Binary</span><span class="sxs-lookup"><span data-stu-id="d5295-116">Binary</span></span>|<span data-ttu-id="d5295-117">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d5295-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="d5295-118">mac</span><span class="sxs-lookup"><span data-stu-id="d5295-118">mac</span></span>|<span data-ttu-id="d5295-119">Binary</span><span class="sxs-lookup"><span data-stu-id="d5295-119">Binary</span></span>|<span data-ttu-id="d5295-120">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="d5295-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="d5295-121">macKey</span><span class="sxs-lookup"><span data-stu-id="d5295-121">macKey</span></span>|<span data-ttu-id="d5295-122">Binary</span><span class="sxs-lookup"><span data-stu-id="d5295-122">Binary</span></span>|<span data-ttu-id="d5295-123">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d5295-123">The key used to get mac.</span></span>|
|<span data-ttu-id="d5295-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5295-124">profileIdentifier</span></span>|<span data-ttu-id="d5295-125">String</span><span class="sxs-lookup"><span data-stu-id="d5295-125">String</span></span>|<span data-ttu-id="d5295-126">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="d5295-126">The the profile identifier.</span></span>|
|<span data-ttu-id="d5295-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="d5295-127">fileDigest</span></span>|<span data-ttu-id="d5295-128">Binary</span><span class="sxs-lookup"><span data-stu-id="d5295-128">Binary</span></span>|<span data-ttu-id="d5295-129">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="d5295-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="d5295-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d5295-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="d5295-131">String</span><span class="sxs-lookup"><span data-stu-id="d5295-131">String</span></span>|<span data-ttu-id="d5295-132">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="d5295-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5295-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d5295-133">Relationships</span></span>
<span data-ttu-id="d5295-134">Keine</span><span class="sxs-lookup"><span data-stu-id="d5295-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5295-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d5295-135">JSON Representation</span></span>
<span data-ttu-id="d5295-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d5295-136">Here is a JSON representation of the resource.</span></span>
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




