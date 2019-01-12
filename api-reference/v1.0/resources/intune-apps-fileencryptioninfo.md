---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5642c76e7d09d1113f2fccc68fc7b1db8ba0ffde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931601"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="96f29-103">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="96f29-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="96f29-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96f29-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96f29-105">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="96f29-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="96f29-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96f29-106">Properties</span></span>
|<span data-ttu-id="96f29-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96f29-107">Property</span></span>|<span data-ttu-id="96f29-108">Typ</span><span class="sxs-lookup"><span data-stu-id="96f29-108">Type</span></span>|<span data-ttu-id="96f29-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96f29-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96f29-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="96f29-110">encryptionKey</span></span>|<span data-ttu-id="96f29-111">Binary</span><span class="sxs-lookup"><span data-stu-id="96f29-111">Binary</span></span>|<span data-ttu-id="96f29-112">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="96f29-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="96f29-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="96f29-113">initializationVector</span></span>|<span data-ttu-id="96f29-114">Binary</span><span class="sxs-lookup"><span data-stu-id="96f29-114">Binary</span></span>|<span data-ttu-id="96f29-115">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="96f29-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="96f29-116">mac</span><span class="sxs-lookup"><span data-stu-id="96f29-116">mac</span></span>|<span data-ttu-id="96f29-117">Binary</span><span class="sxs-lookup"><span data-stu-id="96f29-117">Binary</span></span>|<span data-ttu-id="96f29-118">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="96f29-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="96f29-119">macKey</span><span class="sxs-lookup"><span data-stu-id="96f29-119">macKey</span></span>|<span data-ttu-id="96f29-120">Binary</span><span class="sxs-lookup"><span data-stu-id="96f29-120">Binary</span></span>|<span data-ttu-id="96f29-121">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="96f29-121">The key used to get mac.</span></span>|
|<span data-ttu-id="96f29-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="96f29-122">profileIdentifier</span></span>|<span data-ttu-id="96f29-123">String</span><span class="sxs-lookup"><span data-stu-id="96f29-123">String</span></span>|<span data-ttu-id="96f29-124">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="96f29-124">The the profile identifier.</span></span>|
|<span data-ttu-id="96f29-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="96f29-125">fileDigest</span></span>|<span data-ttu-id="96f29-126">Binary</span><span class="sxs-lookup"><span data-stu-id="96f29-126">Binary</span></span>|<span data-ttu-id="96f29-127">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="96f29-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="96f29-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="96f29-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="96f29-129">String</span><span class="sxs-lookup"><span data-stu-id="96f29-129">String</span></span>|<span data-ttu-id="96f29-130">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="96f29-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96f29-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="96f29-131">Relationships</span></span>
<span data-ttu-id="96f29-132">Keine</span><span class="sxs-lookup"><span data-stu-id="96f29-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96f29-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96f29-133">JSON Representation</span></span>
<span data-ttu-id="96f29-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="96f29-134">Here is a JSON representation of the resource.</span></span>
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



