---
title: Ressourcentyp bitLockerFixedDrivePolicy
description: BitLocker feste Laufwerk Richtlinien.
author: tfitzmac
ms.openlocfilehash: 71fc28fc88689165cdcd187542460432948f78c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342616"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="02b9c-103">Ressourcentyp bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="02b9c-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="02b9c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02b9c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02b9c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02b9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02b9c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="02b9c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02b9c-107">BitLocker feste Laufwerk Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="02b9c-107">BitLocker Fixed Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="02b9c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="02b9c-108">Properties</span></span>
|<span data-ttu-id="02b9c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02b9c-109">Property</span></span>|<span data-ttu-id="02b9c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="02b9c-110">Type</span></span>|<span data-ttu-id="02b9c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02b9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02b9c-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="02b9c-112">encryptionMethod</span></span>|[<span data-ttu-id="02b9c-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="02b9c-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="02b9c-114">Wählen Sie die Verschlüsselungsmethode für Festplatten.</span><span class="sxs-lookup"><span data-stu-id="02b9c-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="02b9c-115">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="02b9c-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="02b9c-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="02b9c-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="02b9c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="02b9c-117">Boolean</span></span>|<span data-ttu-id="02b9c-118">Diese Einstellung bestimmt, ob der BitLocker-Schutz für feste Datenlaufwerke, die auf einem Computer geschrieben werden erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="02b9c-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="02b9c-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="02b9c-119">recoveryOptions</span></span>|[<span data-ttu-id="02b9c-120">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="02b9c-120">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="02b9c-121">Mit dieser richtlinieneinstellung können Sie wie BitLocker-geschützten feste Daten steuern Laufwerke fehlen die erforderlichen Anmeldeinformationen wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="02b9c-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="02b9c-122">Diese Einstellung wird angewendet, wenn Sie BitLocker aktivieren.</span><span class="sxs-lookup"><span data-stu-id="02b9c-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02b9c-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="02b9c-123">Relationships</span></span>
<span data-ttu-id="02b9c-124">Keine</span><span class="sxs-lookup"><span data-stu-id="02b9c-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="02b9c-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="02b9c-125">JSON Representation</span></span>
<span data-ttu-id="02b9c-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="02b9c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```





