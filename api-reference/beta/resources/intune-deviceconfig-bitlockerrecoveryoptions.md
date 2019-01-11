---
title: Ressourcentyp bitLockerRecoveryOptions
description: BitLocker Wiederherstellungsoptionen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eae2052f71d1b1d048072c70dc76437811c1cd8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806454"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="83671-103">Ressourcentyp bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="83671-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="83671-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="83671-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83671-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83671-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83671-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="83671-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83671-107">BitLocker Wiederherstellungsoptionen.</span><span class="sxs-lookup"><span data-stu-id="83671-107">BitLocker Recovery Options.</span></span>
## <a name="properties"></a><span data-ttu-id="83671-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83671-108">Properties</span></span>
|<span data-ttu-id="83671-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83671-109">Property</span></span>|<span data-ttu-id="83671-110">Typ</span><span class="sxs-lookup"><span data-stu-id="83671-110">Type</span></span>|<span data-ttu-id="83671-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83671-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83671-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="83671-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="83671-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="83671-113">Boolean</span></span>|<span data-ttu-id="83671-114">Gibt an, ob zertifikatbasierte Datenwiederherstellungsagent blockiert.</span><span class="sxs-lookup"><span data-stu-id="83671-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="83671-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="83671-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="83671-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="83671-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="83671-117">Gibt an, ob Benutzer zugelassen oder erforderlich, um ein Wiederherstellungskennwort 48 Ziffern generieren für feste oder Systemdatenträger.</span><span class="sxs-lookup"><span data-stu-id="83671-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="83671-118">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="83671-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="83671-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="83671-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="83671-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="83671-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="83671-121">Gibt an, ob Benutzer zugelassen oder erforderlich, um eine 256-Bit-Wiederherstellungsschlüssel generieren für feste oder Systemdatenträger.</span><span class="sxs-lookup"><span data-stu-id="83671-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="83671-122">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="83671-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="83671-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="83671-123">hideRecoveryOptions</span></span>|<span data-ttu-id="83671-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="83671-124">Boolean</span></span>|<span data-ttu-id="83671-125">Gibt an, ob Wiederherstellungsoptionen BitLocker-Setup-Assistenten enthält die feste zulassen oder Systemdatenträger.</span><span class="sxs-lookup"><span data-stu-id="83671-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="83671-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="83671-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="83671-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="83671-127">Boolean</span></span>|<span data-ttu-id="83671-128">Gibt an, ob BitLocker-Wiederherstellungsinformationen in AD DS speichern können.</span><span class="sxs-lookup"><span data-stu-id="83671-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="83671-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="83671-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="83671-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="83671-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="83671-131">Konfigurieren Sie, welche Teile der BitLocker-Wiederherstellungsinformationen in AD DS gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="83671-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="83671-132">Mögliche Werte sind: `passwordAndKey` und `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="83671-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="83671-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="83671-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="83671-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="83671-134">Boolean</span></span>|<span data-ttu-id="83671-135">Gibt an, ob BitLocker aktivieren, bis Wiederherstellungsinformationen in AD DS gespeichert wird.</span><span class="sxs-lookup"><span data-stu-id="83671-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83671-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="83671-136">Relationships</span></span>
<span data-ttu-id="83671-137">Keine</span><span class="sxs-lookup"><span data-stu-id="83671-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="83671-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83671-138">JSON Representation</span></span>
<span data-ttu-id="83671-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83671-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```





