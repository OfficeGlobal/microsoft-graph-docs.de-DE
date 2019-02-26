---
title: bitLockerRemovableDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für Wechseldatenträger.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d10a1039c0186238504836c0f719ab19ae4c4882
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261761"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="8958d-103">bitLockerRemovableDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8958d-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="8958d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8958d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8958d-105">BitLocker-Richtlinien für Wechseldatenträger.</span><span class="sxs-lookup"><span data-stu-id="8958d-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="8958d-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8958d-106">Properties</span></span>
|<span data-ttu-id="8958d-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8958d-107">Property</span></span>|<span data-ttu-id="8958d-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8958d-108">Type</span></span>|<span data-ttu-id="8958d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8958d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8958d-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="8958d-110">encryptionMethod</span></span>|[<span data-ttu-id="8958d-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="8958d-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="8958d-112">Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus.</span><span class="sxs-lookup"><span data-stu-id="8958d-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="8958d-113">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="8958d-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="8958d-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="8958d-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="8958d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8958d-115">Boolean</span></span>|<span data-ttu-id="8958d-116">Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="8958d-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="8958d-117">Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="8958d-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="8958d-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="8958d-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="8958d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8958d-119">Boolean</span></span>|<span data-ttu-id="8958d-120">Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="8958d-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8958d-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8958d-121">Relationships</span></span>
<span data-ttu-id="8958d-122">Keine</span><span class="sxs-lookup"><span data-stu-id="8958d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8958d-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8958d-123">JSON Representation</span></span>
<span data-ttu-id="8958d-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8958d-124">Here is a JSON representation of the resource.</span></span>
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



