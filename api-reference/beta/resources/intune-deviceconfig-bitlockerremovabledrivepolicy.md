---
title: bitLockerRemovableDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für Wechseldatenträger.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57a3ad19e988327e126b6da757c2dc5b90c280de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425617"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="d0c32-103">bitLockerRemovableDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0c32-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="d0c32-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d0c32-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0c32-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0c32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0c32-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0c32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0c32-107">BitLocker-Richtlinien für Wechseldatenträger.</span><span class="sxs-lookup"><span data-stu-id="d0c32-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="d0c32-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0c32-108">Properties</span></span>
|<span data-ttu-id="d0c32-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0c32-109">Property</span></span>|<span data-ttu-id="d0c32-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d0c32-110">Type</span></span>|<span data-ttu-id="d0c32-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0c32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0c32-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d0c32-112">encryptionMethod</span></span>|[<span data-ttu-id="d0c32-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d0c32-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="d0c32-114">Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus.</span><span class="sxs-lookup"><span data-stu-id="d0c32-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="d0c32-115">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="d0c32-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="d0c32-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="d0c32-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="d0c32-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0c32-117">Boolean</span></span>|<span data-ttu-id="d0c32-118">Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="d0c32-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="d0c32-119">Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="d0c32-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="d0c32-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="d0c32-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="d0c32-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0c32-121">Boolean</span></span>|<span data-ttu-id="d0c32-122">Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="d0c32-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0c32-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d0c32-123">Relationships</span></span>
<span data-ttu-id="d0c32-124">Keine</span><span class="sxs-lookup"><span data-stu-id="d0c32-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0c32-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d0c32-125">JSON Representation</span></span>
<span data-ttu-id="d0c32-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d0c32-126">Here is a JSON representation of the resource.</span></span>
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




