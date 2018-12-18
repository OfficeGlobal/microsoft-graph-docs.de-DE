---
title: bitLockerRemovableDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für Wechseldatenträger.
author: tfitzmac
ms.openlocfilehash: 15de11384195350b455cd4696a260aedf1de7a26
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354034"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="340d6-103">bitLockerRemovableDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="340d6-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="340d6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="340d6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="340d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="340d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="340d6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="340d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="340d6-107">BitLocker-Richtlinien für Wechseldatenträger.</span><span class="sxs-lookup"><span data-stu-id="340d6-107">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="340d6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="340d6-108">Properties</span></span>
|<span data-ttu-id="340d6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="340d6-109">Property</span></span>|<span data-ttu-id="340d6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="340d6-110">Type</span></span>|<span data-ttu-id="340d6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="340d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="340d6-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="340d6-112">encryptionMethod</span></span>|[<span data-ttu-id="340d6-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="340d6-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="340d6-114">Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus.</span><span class="sxs-lookup"><span data-stu-id="340d6-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="340d6-115">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="340d6-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="340d6-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="340d6-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="340d6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="340d6-117">Boolean</span></span>|<span data-ttu-id="340d6-118">Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="340d6-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="340d6-119">Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="340d6-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="340d6-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="340d6-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="340d6-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="340d6-121">Boolean</span></span>|<span data-ttu-id="340d6-122">Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="340d6-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="340d6-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="340d6-123">Relationships</span></span>
<span data-ttu-id="340d6-124">Keine</span><span class="sxs-lookup"><span data-stu-id="340d6-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="340d6-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="340d6-125">JSON Representation</span></span>
<span data-ttu-id="340d6-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="340d6-126">Here is a JSON representation of the resource.</span></span>
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





