---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
ms.openlocfilehash: 17895b0bf081cc249f9081c737a2445683514280
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059191"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="d8ca6-103">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d8ca6-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="d8ca6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8ca6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8ca6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8ca6-107">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="d8ca6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d8ca6-108">Properties</span></span>
|<span data-ttu-id="d8ca6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d8ca6-109">Property</span></span>|<span data-ttu-id="d8ca6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d8ca6-110">Type</span></span>|<span data-ttu-id="d8ca6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8ca6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8ca6-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="d8ca6-112">encryptionKey</span></span>|<span data-ttu-id="d8ca6-113">Binary</span><span class="sxs-lookup"><span data-stu-id="d8ca6-113">Binary</span></span>|<span data-ttu-id="d8ca6-114">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="d8ca6-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="d8ca6-115">initializationVector</span></span>|<span data-ttu-id="d8ca6-116">Binary</span><span class="sxs-lookup"><span data-stu-id="d8ca6-116">Binary</span></span>|<span data-ttu-id="d8ca6-117">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="d8ca6-118">mac</span><span class="sxs-lookup"><span data-stu-id="d8ca6-118">mac</span></span>|<span data-ttu-id="d8ca6-119">Binary</span><span class="sxs-lookup"><span data-stu-id="d8ca6-119">Binary</span></span>|<span data-ttu-id="d8ca6-120">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="d8ca6-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="d8ca6-121">macKey</span><span class="sxs-lookup"><span data-stu-id="d8ca6-121">macKey</span></span>|<span data-ttu-id="d8ca6-122">Binary</span><span class="sxs-lookup"><span data-stu-id="d8ca6-122">Binary</span></span>|<span data-ttu-id="d8ca6-123">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-123">The key used to get mac.</span></span>|
|<span data-ttu-id="d8ca6-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="d8ca6-124">profileIdentifier</span></span>|<span data-ttu-id="d8ca6-125">String</span><span class="sxs-lookup"><span data-stu-id="d8ca6-125">String</span></span>|<span data-ttu-id="d8ca6-126">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-126">The the profile identifier.</span></span>|
|<span data-ttu-id="d8ca6-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="d8ca6-127">fileDigest</span></span>|<span data-ttu-id="d8ca6-128">Binary</span><span class="sxs-lookup"><span data-stu-id="d8ca6-128">Binary</span></span>|<span data-ttu-id="d8ca6-129">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="d8ca6-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d8ca6-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="d8ca6-131">String</span><span class="sxs-lookup"><span data-stu-id="d8ca6-131">String</span></span>|<span data-ttu-id="d8ca6-132">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8ca6-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d8ca6-133">Relationships</span></span>
<span data-ttu-id="d8ca6-134">Keine</span><span class="sxs-lookup"><span data-stu-id="d8ca6-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d8ca6-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d8ca6-135">JSON Representation</span></span>
<span data-ttu-id="d8ca6-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d8ca6-136">Here is a JSON representation of the resource.</span></span>
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





