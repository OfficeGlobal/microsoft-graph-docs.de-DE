---
title: bitLockerRemovableDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für Wechseldatenträger.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fc9fe3350fd9f4b5c5808de2c35fa3451943e449
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830835"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="ffc08-103">bitLockerRemovableDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ffc08-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="ffc08-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ffc08-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffc08-105">BitLocker-Richtlinien für Wechseldatenträger.</span><span class="sxs-lookup"><span data-stu-id="ffc08-105">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="ffc08-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ffc08-106">Properties</span></span>
|<span data-ttu-id="ffc08-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ffc08-107">Property</span></span>|<span data-ttu-id="ffc08-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ffc08-108">Type</span></span>|<span data-ttu-id="ffc08-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffc08-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffc08-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="ffc08-110">encryptionMethod</span></span>|[<span data-ttu-id="ffc08-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="ffc08-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="ffc08-112">Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus.</span><span class="sxs-lookup"><span data-stu-id="ffc08-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="ffc08-113">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="ffc08-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="ffc08-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="ffc08-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="ffc08-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffc08-115">Boolean</span></span>|<span data-ttu-id="ffc08-116">Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="ffc08-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="ffc08-117">Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="ffc08-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="ffc08-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="ffc08-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="ffc08-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffc08-119">Boolean</span></span>|<span data-ttu-id="ffc08-120">Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="ffc08-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffc08-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ffc08-121">Relationships</span></span>
<span data-ttu-id="ffc08-122">Keine</span><span class="sxs-lookup"><span data-stu-id="ffc08-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ffc08-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ffc08-123">JSON Representation</span></span>
<span data-ttu-id="ffc08-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ffc08-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



