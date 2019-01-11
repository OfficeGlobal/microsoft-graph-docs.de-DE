---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 03d8adbbf43b38bfc7d13bec2db09c2be8c3b2ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868971"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="23ede-103">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="23ede-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="23ede-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23ede-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23ede-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23ede-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23ede-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23ede-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23ede-107">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="23ede-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="23ede-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23ede-108">Properties</span></span>
|<span data-ttu-id="23ede-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23ede-109">Property</span></span>|<span data-ttu-id="23ede-110">Typ</span><span class="sxs-lookup"><span data-stu-id="23ede-110">Type</span></span>|<span data-ttu-id="23ede-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23ede-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23ede-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="23ede-112">encryptionKey</span></span>|<span data-ttu-id="23ede-113">Binary</span><span class="sxs-lookup"><span data-stu-id="23ede-113">Binary</span></span>|<span data-ttu-id="23ede-114">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="23ede-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="23ede-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="23ede-115">initializationVector</span></span>|<span data-ttu-id="23ede-116">Binary</span><span class="sxs-lookup"><span data-stu-id="23ede-116">Binary</span></span>|<span data-ttu-id="23ede-117">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="23ede-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="23ede-118">mac</span><span class="sxs-lookup"><span data-stu-id="23ede-118">mac</span></span>|<span data-ttu-id="23ede-119">Binary</span><span class="sxs-lookup"><span data-stu-id="23ede-119">Binary</span></span>|<span data-ttu-id="23ede-120">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="23ede-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="23ede-121">macKey</span><span class="sxs-lookup"><span data-stu-id="23ede-121">macKey</span></span>|<span data-ttu-id="23ede-122">Binary</span><span class="sxs-lookup"><span data-stu-id="23ede-122">Binary</span></span>|<span data-ttu-id="23ede-123">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="23ede-123">The key used to get mac.</span></span>|
|<span data-ttu-id="23ede-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="23ede-124">profileIdentifier</span></span>|<span data-ttu-id="23ede-125">String</span><span class="sxs-lookup"><span data-stu-id="23ede-125">String</span></span>|<span data-ttu-id="23ede-126">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="23ede-126">The the profile identifier.</span></span>|
|<span data-ttu-id="23ede-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="23ede-127">fileDigest</span></span>|<span data-ttu-id="23ede-128">Binary</span><span class="sxs-lookup"><span data-stu-id="23ede-128">Binary</span></span>|<span data-ttu-id="23ede-129">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="23ede-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="23ede-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="23ede-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="23ede-131">String</span><span class="sxs-lookup"><span data-stu-id="23ede-131">String</span></span>|<span data-ttu-id="23ede-132">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="23ede-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23ede-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23ede-133">Relationships</span></span>
<span data-ttu-id="23ede-134">Keine</span><span class="sxs-lookup"><span data-stu-id="23ede-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23ede-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23ede-135">JSON Representation</span></span>
<span data-ttu-id="23ede-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23ede-136">Here is a JSON representation of the resource.</span></span>
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





