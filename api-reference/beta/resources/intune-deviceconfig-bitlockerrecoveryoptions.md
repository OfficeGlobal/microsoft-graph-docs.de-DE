---
title: bitLockerRecoveryOptions-Ressourcentyp
description: BitLocker-wiederHerstellungsOptionen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8bbf0db0ca6dd784a47d1bfb5d743ae17695b81
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142112"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="50e8a-103">bitLockerRecoveryOptions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="50e8a-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="50e8a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50e8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50e8a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="50e8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50e8a-106">BitLocker-wiederHerstellungsOptionen.</span><span class="sxs-lookup"><span data-stu-id="50e8a-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="50e8a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50e8a-107">Properties</span></span>
|<span data-ttu-id="50e8a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50e8a-108">Property</span></span>|<span data-ttu-id="50e8a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="50e8a-109">Type</span></span>|<span data-ttu-id="50e8a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50e8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50e8a-111">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="50e8a-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="50e8a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e8a-112">Boolean</span></span>|<span data-ttu-id="50e8a-113">Gibt an, ob der zertifikatbasierte Daten Wiederherstellungs-Agent blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="50e8a-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="50e8a-114">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="50e8a-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="50e8a-115">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="50e8a-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="50e8a-116">Gibt an, ob Benutzer zum Generieren eines 48-stelligen Wiederherstellungskennworts für den fest-oder Systemdatenträger berechtigt oder erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="50e8a-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="50e8a-117">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="50e8a-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="50e8a-118">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="50e8a-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="50e8a-119">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="50e8a-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="50e8a-120">Gibt an, ob Benutzer zulässig oder erforderlich sind, um einen 256-Bit-Wiederherstellungsschlüssel für feste oder Systemdatenträger zu generieren.</span><span class="sxs-lookup"><span data-stu-id="50e8a-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="50e8a-121">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="50e8a-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="50e8a-122">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="50e8a-122">hideRecoveryOptions</span></span>|<span data-ttu-id="50e8a-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e8a-123">Boolean</span></span>|<span data-ttu-id="50e8a-124">Gibt an, ob das Anzeigen von Wiederherstellungsoptionen im BitLocker-Setup-Assistenten für feste oder Systemdatenträger zugelassen werden soll.</span><span class="sxs-lookup"><span data-stu-id="50e8a-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="50e8a-125">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="50e8a-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="50e8a-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e8a-126">Boolean</span></span>|<span data-ttu-id="50e8a-127">Gibt an, ob BitLocker-Wiederherstellungsinformationen in AD DS gespeichert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="50e8a-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="50e8a-128">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="50e8a-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="50e8a-129">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="50e8a-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="50e8a-130">Konfigurieren Sie, welche Teile von BitLocker-Wiederherstellungsinformationen in AD DS gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="50e8a-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="50e8a-131">Mögliche Werte sind: `passwordAndKey` und `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="50e8a-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="50e8a-132">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="50e8a-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="50e8a-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e8a-133">Boolean</span></span>|<span data-ttu-id="50e8a-134">Gibt an, ob BitLocker aktiviert werden soll, bis Wiederherstellungsinformationen in AD DS gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="50e8a-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50e8a-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="50e8a-135">Relationships</span></span>
<span data-ttu-id="50e8a-136">Keine</span><span class="sxs-lookup"><span data-stu-id="50e8a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50e8a-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50e8a-137">JSON Representation</span></span>
<span data-ttu-id="50e8a-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50e8a-138">Here is a JSON representation of the resource.</span></span>
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




