---
title: bitLockerRemovableDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für Wechseldatenträger.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e7e343fc32af61b38c1cd14cf1fba29de549e99
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149427"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="85e44-103">bitLockerRemovableDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="85e44-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="85e44-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85e44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85e44-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="85e44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e44-106">BitLocker-Richtlinien für Wechseldatenträger.</span><span class="sxs-lookup"><span data-stu-id="85e44-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="85e44-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85e44-107">Properties</span></span>
|<span data-ttu-id="85e44-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85e44-108">Property</span></span>|<span data-ttu-id="85e44-109">Typ</span><span class="sxs-lookup"><span data-stu-id="85e44-109">Type</span></span>|<span data-ttu-id="85e44-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85e44-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e44-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="85e44-111">encryptionMethod</span></span>|[<span data-ttu-id="85e44-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="85e44-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="85e44-113">Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus.</span><span class="sxs-lookup"><span data-stu-id="85e44-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="85e44-114">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="85e44-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="85e44-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="85e44-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="85e44-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e44-116">Boolean</span></span>|<span data-ttu-id="85e44-117">Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="85e44-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="85e44-118">Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="85e44-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="85e44-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="85e44-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="85e44-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e44-120">Boolean</span></span>|<span data-ttu-id="85e44-121">Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="85e44-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85e44-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="85e44-122">Relationships</span></span>
<span data-ttu-id="85e44-123">Keine</span><span class="sxs-lookup"><span data-stu-id="85e44-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85e44-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85e44-124">JSON Representation</span></span>
<span data-ttu-id="85e44-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="85e44-125">Here is a JSON representation of the resource.</span></span>
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




