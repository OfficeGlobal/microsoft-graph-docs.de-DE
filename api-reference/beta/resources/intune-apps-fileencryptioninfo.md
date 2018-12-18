---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
author: tfitzmac
ms.openlocfilehash: a13c451193d248d09e020cc6b308b9f03d991295
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307854"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="807d8-103">fileEncryptionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="807d8-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="807d8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="807d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="807d8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="807d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="807d8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="807d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="807d8-107">Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.</span><span class="sxs-lookup"><span data-stu-id="807d8-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="807d8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="807d8-108">Properties</span></span>
|<span data-ttu-id="807d8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="807d8-109">Property</span></span>|<span data-ttu-id="807d8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="807d8-110">Type</span></span>|<span data-ttu-id="807d8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="807d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="807d8-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="807d8-112">encryptionKey</span></span>|<span data-ttu-id="807d8-113">Binary</span><span class="sxs-lookup"><span data-stu-id="807d8-113">Binary</span></span>|<span data-ttu-id="807d8-114">Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="807d8-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="807d8-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="807d8-115">initializationVector</span></span>|<span data-ttu-id="807d8-116">Binary</span><span class="sxs-lookup"><span data-stu-id="807d8-116">Binary</span></span>|<span data-ttu-id="807d8-117">Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="807d8-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="807d8-118">mac</span><span class="sxs-lookup"><span data-stu-id="807d8-118">mac</span></span>|<span data-ttu-id="807d8-119">Binary</span><span class="sxs-lookup"><span data-stu-id="807d8-119">Binary</span></span>|<span data-ttu-id="807d8-120">Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).</span><span class="sxs-lookup"><span data-stu-id="807d8-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="807d8-121">macKey</span><span class="sxs-lookup"><span data-stu-id="807d8-121">macKey</span></span>|<span data-ttu-id="807d8-122">Binary</span><span class="sxs-lookup"><span data-stu-id="807d8-122">Binary</span></span>|<span data-ttu-id="807d8-123">Der Schlüssel, der für den Abruf von mac verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="807d8-123">The key used to get mac.</span></span>|
|<span data-ttu-id="807d8-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="807d8-124">profileIdentifier</span></span>|<span data-ttu-id="807d8-125">String</span><span class="sxs-lookup"><span data-stu-id="807d8-125">String</span></span>|<span data-ttu-id="807d8-126">Die Bezeichner des Profils.</span><span class="sxs-lookup"><span data-stu-id="807d8-126">The the profile identifier.</span></span>|
|<span data-ttu-id="807d8-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="807d8-127">fileDigest</span></span>|<span data-ttu-id="807d8-128">Binary</span><span class="sxs-lookup"><span data-stu-id="807d8-128">Binary</span></span>|<span data-ttu-id="807d8-129">Der Digest der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="807d8-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="807d8-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="807d8-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="807d8-131">String</span><span class="sxs-lookup"><span data-stu-id="807d8-131">String</span></span>|<span data-ttu-id="807d8-132">Der Dateidigestalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="807d8-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="807d8-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="807d8-133">Relationships</span></span>
<span data-ttu-id="807d8-134">Keine</span><span class="sxs-lookup"><span data-stu-id="807d8-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="807d8-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="807d8-135">JSON Representation</span></span>
<span data-ttu-id="807d8-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="807d8-136">Here is a JSON representation of the resource.</span></span>
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





