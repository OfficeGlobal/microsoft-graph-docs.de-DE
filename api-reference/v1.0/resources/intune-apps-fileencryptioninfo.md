---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
author: tfitzmac
ms.openlocfilehash: c58865e746afcde8167c8d905c3b4064d8690a95
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309184"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="aca0b-103">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aca0b-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="aca0b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aca0b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aca0b-105">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="aca0b-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="aca0b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aca0b-106">Properties</span></span>
|<span data-ttu-id="aca0b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aca0b-107">Property</span></span>|<span data-ttu-id="aca0b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="aca0b-108">Type</span></span>|<span data-ttu-id="aca0b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aca0b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aca0b-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="aca0b-110">encryptionKey</span></span>|<span data-ttu-id="aca0b-111">Binary</span><span class="sxs-lookup"><span data-stu-id="aca0b-111">Binary</span></span>|<span data-ttu-id="aca0b-112">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="aca0b-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="aca0b-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="aca0b-113">initializationVector</span></span>|<span data-ttu-id="aca0b-114">Binary</span><span class="sxs-lookup"><span data-stu-id="aca0b-114">Binary</span></span>|<span data-ttu-id="aca0b-115">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="aca0b-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="aca0b-116">mac</span><span class="sxs-lookup"><span data-stu-id="aca0b-116">mac</span></span>|<span data-ttu-id="aca0b-117">Binary</span><span class="sxs-lookup"><span data-stu-id="aca0b-117">Binary</span></span>|<span data-ttu-id="aca0b-118">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="aca0b-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="aca0b-119">macKey</span><span class="sxs-lookup"><span data-stu-id="aca0b-119">macKey</span></span>|<span data-ttu-id="aca0b-120">Binary</span><span class="sxs-lookup"><span data-stu-id="aca0b-120">Binary</span></span>|<span data-ttu-id="aca0b-121">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="aca0b-121">The key used to get mac.</span></span>|
|<span data-ttu-id="aca0b-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="aca0b-122">profileIdentifier</span></span>|<span data-ttu-id="aca0b-123">String</span><span class="sxs-lookup"><span data-stu-id="aca0b-123">String</span></span>|<span data-ttu-id="aca0b-124">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="aca0b-124">The the profile identifier.</span></span>|
|<span data-ttu-id="aca0b-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="aca0b-125">fileDigest</span></span>|<span data-ttu-id="aca0b-126">Binary</span><span class="sxs-lookup"><span data-stu-id="aca0b-126">Binary</span></span>|<span data-ttu-id="aca0b-127">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="aca0b-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="aca0b-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="aca0b-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="aca0b-129">String</span><span class="sxs-lookup"><span data-stu-id="aca0b-129">String</span></span>|<span data-ttu-id="aca0b-130">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="aca0b-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aca0b-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aca0b-131">Relationships</span></span>
<span data-ttu-id="aca0b-132">Keine</span><span class="sxs-lookup"><span data-stu-id="aca0b-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aca0b-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aca0b-133">JSON Representation</span></span>
<span data-ttu-id="aca0b-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aca0b-134">Here is a JSON representation of the resource.</span></span>
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



