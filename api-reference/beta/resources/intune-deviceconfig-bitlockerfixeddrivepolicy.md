---
title: Ressourcentyp bitLockerFixedDrivePolicy
description: BitLocker feste Laufwerk Richtlinien.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8f233e4c1779a860cc40dc97007aa0216795928f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424665"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="5be29-103">Ressourcentyp bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5be29-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="5be29-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5be29-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5be29-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5be29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5be29-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5be29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5be29-107">BitLocker feste Laufwerk Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="5be29-107">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="5be29-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5be29-108">Properties</span></span>
|<span data-ttu-id="5be29-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5be29-109">Property</span></span>|<span data-ttu-id="5be29-110">Typ</span><span class="sxs-lookup"><span data-stu-id="5be29-110">Type</span></span>|<span data-ttu-id="5be29-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5be29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5be29-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="5be29-112">encryptionMethod</span></span>|[<span data-ttu-id="5be29-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="5be29-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="5be29-114">Wählen Sie die Verschlüsselungsmethode für Festplatten.</span><span class="sxs-lookup"><span data-stu-id="5be29-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="5be29-115">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="5be29-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="5be29-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="5be29-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="5be29-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="5be29-117">Boolean</span></span>|<span data-ttu-id="5be29-118">Diese Einstellung bestimmt, ob der BitLocker-Schutz für feste Datenlaufwerke, die auf einem Computer geschrieben werden erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="5be29-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="5be29-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="5be29-119">recoveryOptions</span></span>|[<span data-ttu-id="5be29-120">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="5be29-120">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="5be29-121">Mit dieser richtlinieneinstellung können Sie wie BitLocker-geschützten feste Daten steuern Laufwerke fehlen die erforderlichen Anmeldeinformationen wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="5be29-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="5be29-122">Diese Einstellung wird angewendet, wenn Sie BitLocker aktivieren.</span><span class="sxs-lookup"><span data-stu-id="5be29-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5be29-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5be29-123">Relationships</span></span>
<span data-ttu-id="5be29-124">Keine</span><span class="sxs-lookup"><span data-stu-id="5be29-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5be29-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5be29-125">JSON Representation</span></span>
<span data-ttu-id="5be29-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5be29-126">Here is a JSON representation of the resource.</span></span>
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




