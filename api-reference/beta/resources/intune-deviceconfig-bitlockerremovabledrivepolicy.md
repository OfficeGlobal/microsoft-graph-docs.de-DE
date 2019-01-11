---
title: bitLockerRemovableDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für Wechseldatenträger.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b5c7d0d7fc188ee0c150bb7d0ac2143639ca32ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873983"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="45365-103">bitLockerRemovableDrivePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="45365-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="45365-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="45365-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45365-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="45365-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45365-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="45365-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45365-107">BitLocker-Richtlinien für Wechseldatenträger.</span><span class="sxs-lookup"><span data-stu-id="45365-107">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="45365-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="45365-108">Properties</span></span>
|<span data-ttu-id="45365-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45365-109">Property</span></span>|<span data-ttu-id="45365-110">Typ</span><span class="sxs-lookup"><span data-stu-id="45365-110">Type</span></span>|<span data-ttu-id="45365-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45365-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45365-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="45365-112">encryptionMethod</span></span>|[<span data-ttu-id="45365-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="45365-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="45365-114">Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus.</span><span class="sxs-lookup"><span data-stu-id="45365-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="45365-115">Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="45365-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="45365-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="45365-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="45365-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="45365-117">Boolean</span></span>|<span data-ttu-id="45365-118">Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="45365-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="45365-119">Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.</span><span class="sxs-lookup"><span data-stu-id="45365-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="45365-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="45365-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="45365-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="45365-121">Boolean</span></span>|<span data-ttu-id="45365-122">Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.</span><span class="sxs-lookup"><span data-stu-id="45365-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45365-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="45365-123">Relationships</span></span>
<span data-ttu-id="45365-124">Keine</span><span class="sxs-lookup"><span data-stu-id="45365-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="45365-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="45365-125">JSON Representation</span></span>
<span data-ttu-id="45365-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="45365-126">Here is a JSON representation of the resource.</span></span>
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





