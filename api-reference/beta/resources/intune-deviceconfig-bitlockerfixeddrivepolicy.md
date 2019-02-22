---
title: bitLockerFixedDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für feste Laufwerke.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e09130a2426f6a7196d472a29f7667b9c044d313
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164295"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="83a88-103">bitLockerFixedDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="83a88-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="83a88-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83a88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83a88-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="83a88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83a88-106">BitLocker-Richtlinien für feste Laufwerke.</span><span class="sxs-lookup"><span data-stu-id="83a88-106">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="83a88-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83a88-107">Properties</span></span>
|<span data-ttu-id="83a88-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83a88-108">Property</span></span>|<span data-ttu-id="83a88-109">Typ</span><span class="sxs-lookup"><span data-stu-id="83a88-109">Type</span></span>|<span data-ttu-id="83a88-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83a88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83a88-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="83a88-111">encryptionMethod</span></span>|[<span data-ttu-id="83a88-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="83a88-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="83a88-113">Wählen Sie die Verschlüsselungsmethode für feste Laufwerke aus.</span><span class="sxs-lookup"><span data-stu-id="83a88-113">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="83a88-114">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="83a88-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="83a88-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="83a88-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="83a88-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="83a88-116">Boolean</span></span>|<span data-ttu-id="83a88-117">Diese Richtlinieneinstellung bestimmt, ob BitLocker-Schutz erforderlich ist, damit feste Datenlaufwerke auf einem Computer schreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="83a88-117">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="83a88-118">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="83a88-118">recoveryOptions</span></span>|[<span data-ttu-id="83a88-119">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="83a88-119">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="83a88-120">Mit dieser Richtlinieneinstellung können Sie steuern, wie mit BitLocker geschützte feste Datenlaufwerke in Abwesenheit der erforderlichen Anmeldeinformationen wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="83a88-120">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="83a88-121">Diese Richtlinieneinstellung wird angewendet, wenn Sie BitLocker aktivieren.</span><span class="sxs-lookup"><span data-stu-id="83a88-121">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83a88-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="83a88-122">Relationships</span></span>
<span data-ttu-id="83a88-123">Keine</span><span class="sxs-lookup"><span data-stu-id="83a88-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83a88-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83a88-124">JSON Representation</span></span>
<span data-ttu-id="83a88-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83a88-125">Here is a JSON representation of the resource.</span></span>
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




