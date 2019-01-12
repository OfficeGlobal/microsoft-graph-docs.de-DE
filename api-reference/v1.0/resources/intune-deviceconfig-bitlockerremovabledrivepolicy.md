---
title: bitLockerRemovableDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für Wechseldatenträger.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 040f4230cf1d3aab02f97237b88093126f8dc24c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926337"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="e0052-103">bitLockerRemovableDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e0052-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="e0052-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e0052-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0052-105">BitLocker-Richtlinien für Wechseldatenträger.</span><span class="sxs-lookup"><span data-stu-id="e0052-105">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="e0052-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0052-106">Properties</span></span>
|<span data-ttu-id="e0052-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0052-107">Property</span></span>|<span data-ttu-id="e0052-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e0052-108">Type</span></span>|<span data-ttu-id="e0052-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0052-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0052-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e0052-110">encryptionMethod</span></span>|[<span data-ttu-id="e0052-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e0052-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="e0052-112">Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus.</span><span class="sxs-lookup"><span data-stu-id="e0052-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="e0052-113">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="e0052-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="e0052-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="e0052-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="e0052-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0052-115">Boolean</span></span>|<span data-ttu-id="e0052-116">Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="e0052-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="e0052-117">Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="e0052-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="e0052-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="e0052-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="e0052-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0052-119">Boolean</span></span>|<span data-ttu-id="e0052-120">Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="e0052-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0052-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e0052-121">Relationships</span></span>
<span data-ttu-id="e0052-122">Keine</span><span class="sxs-lookup"><span data-stu-id="e0052-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0052-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0052-123">JSON Representation</span></span>
<span data-ttu-id="e0052-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e0052-124">Here is a JSON representation of the resource.</span></span>
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



