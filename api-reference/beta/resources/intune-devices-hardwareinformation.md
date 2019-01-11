---
title: Ressourcentyp hardwareInformation
description: Hardwareinformationen für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2684f1ff7e7a6407942ac61fae7d45ead16820d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831823"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="24494-103">Ressourcentyp hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="24494-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="24494-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="24494-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24494-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24494-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24494-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="24494-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24494-107">Hardwareinformationen für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="24494-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="24494-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="24494-108">Properties</span></span>
|<span data-ttu-id="24494-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24494-109">Property</span></span>|<span data-ttu-id="24494-110">Typ</span><span class="sxs-lookup"><span data-stu-id="24494-110">Type</span></span>|<span data-ttu-id="24494-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24494-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24494-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="24494-112">serialNumber</span></span>|<span data-ttu-id="24494-113">String</span><span class="sxs-lookup"><span data-stu-id="24494-113">String</span></span>|<span data-ttu-id="24494-114">Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="24494-114">Serial number.</span></span>|
|<span data-ttu-id="24494-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="24494-115">totalStorageSpace</span></span>|<span data-ttu-id="24494-116">Int64</span><span class="sxs-lookup"><span data-stu-id="24494-116">Int64</span></span>|<span data-ttu-id="24494-117">Gesamtmenge des Speicherplatzes des Geräts.</span><span class="sxs-lookup"><span data-stu-id="24494-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="24494-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="24494-118">freeStorageSpace</span></span>|<span data-ttu-id="24494-119">Int64</span><span class="sxs-lookup"><span data-stu-id="24494-119">Int64</span></span>|<span data-ttu-id="24494-120">Freier Speicherplatz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="24494-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="24494-121">imei</span><span class="sxs-lookup"><span data-stu-id="24494-121">imei</span></span>|<span data-ttu-id="24494-122">String</span><span class="sxs-lookup"><span data-stu-id="24494-122">String</span></span>|<span data-ttu-id="24494-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="24494-123">IMEI</span></span>|
|<span data-ttu-id="24494-124">meid</span><span class="sxs-lookup"><span data-stu-id="24494-124">meid</span></span>|<span data-ttu-id="24494-125">String</span><span class="sxs-lookup"><span data-stu-id="24494-125">String</span></span>|<span data-ttu-id="24494-126">MEID</span><span class="sxs-lookup"><span data-stu-id="24494-126">MEID</span></span>|
|<span data-ttu-id="24494-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="24494-127">manufacturer</span></span>|<span data-ttu-id="24494-128">String</span><span class="sxs-lookup"><span data-stu-id="24494-128">String</span></span>|<span data-ttu-id="24494-129">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="24494-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="24494-130">model</span><span class="sxs-lookup"><span data-stu-id="24494-130">model</span></span>|<span data-ttu-id="24494-131">String</span><span class="sxs-lookup"><span data-stu-id="24494-131">String</span></span>|<span data-ttu-id="24494-132">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="24494-132">Model of the device</span></span>|
|<span data-ttu-id="24494-133">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="24494-133">phoneNumber</span></span>|<span data-ttu-id="24494-134">String</span><span class="sxs-lookup"><span data-stu-id="24494-134">String</span></span>|<span data-ttu-id="24494-135">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="24494-135">Phone number of the device</span></span>|
|<span data-ttu-id="24494-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="24494-136">subscriberCarrier</span></span>|<span data-ttu-id="24494-137">String</span><span class="sxs-lookup"><span data-stu-id="24494-137">String</span></span>|<span data-ttu-id="24494-138">Abonnenten Netzbetreiber des Geräts</span><span class="sxs-lookup"><span data-stu-id="24494-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="24494-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="24494-139">cellularTechnology</span></span>|<span data-ttu-id="24494-140">String</span><span class="sxs-lookup"><span data-stu-id="24494-140">String</span></span>|<span data-ttu-id="24494-141">Mobilfunk-Technologie des Geräts</span><span class="sxs-lookup"><span data-stu-id="24494-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="24494-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="24494-142">wifiMac</span></span>|<span data-ttu-id="24494-143">String</span><span class="sxs-lookup"><span data-stu-id="24494-143">String</span></span>|<span data-ttu-id="24494-144">WLAN-MAC-Adresse des Geräts</span><span class="sxs-lookup"><span data-stu-id="24494-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="24494-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="24494-145">operatingSystemLanguage</span></span>|<span data-ttu-id="24494-146">String</span><span class="sxs-lookup"><span data-stu-id="24494-146">String</span></span>|<span data-ttu-id="24494-147">Die Sprache des Betriebssystems des Geräts</span><span class="sxs-lookup"><span data-stu-id="24494-147">Operating system language of the device</span></span>|
|<span data-ttu-id="24494-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="24494-148">isSupervised</span></span>|<span data-ttu-id="24494-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="24494-149">Boolean</span></span>|<span data-ttu-id="24494-150">Überwachten Modus des Geräts</span><span class="sxs-lookup"><span data-stu-id="24494-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="24494-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="24494-151">isEncrypted</span></span>|<span data-ttu-id="24494-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="24494-152">Boolean</span></span>|<span data-ttu-id="24494-153">Status der Verschlüsselung des Geräts</span><span class="sxs-lookup"><span data-stu-id="24494-153">Encryption status of the device</span></span>|
|<span data-ttu-id="24494-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="24494-154">isSharedDevice</span></span>|<span data-ttu-id="24494-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="24494-155">Boolean</span></span>|<span data-ttu-id="24494-156">Freigegebene iPad</span><span class="sxs-lookup"><span data-stu-id="24494-156">Shared iPad</span></span>|
|<span data-ttu-id="24494-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="24494-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="24494-158">[SharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="24494-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="24494-159">Alle Benutzer auf dem freigegebenen Apple-Gerät</span><span class="sxs-lookup"><span data-stu-id="24494-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="24494-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="24494-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="24494-161">String</span><span class="sxs-lookup"><span data-stu-id="24494-161">String</span></span>|<span data-ttu-id="24494-162">Zeichenfolge, die die Spezifikation, Version angibt.</span><span class="sxs-lookup"><span data-stu-id="24494-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="24494-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="24494-163">operatingSystemEdition</span></span>|<span data-ttu-id="24494-164">String</span><span class="sxs-lookup"><span data-stu-id="24494-164">String</span></span>|<span data-ttu-id="24494-165">Zeichenfolge, die die Betriebssystem Edition angibt.</span><span class="sxs-lookup"><span data-stu-id="24494-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="24494-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="24494-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="24494-167">String</span><span class="sxs-lookup"><span data-stu-id="24494-167">String</span></span>|<span data-ttu-id="24494-168">Gibt den vollqualifizierten Domänennamen des Geräts (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="24494-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="24494-169">Wenn das Gerät nicht Mitglied einer Domäne ist, wird eine leere Zeichenfolge zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24494-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="24494-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="24494-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="24494-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="24494-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="24494-172">Virtualisierung-basierte Hardware Anforderung Sicherheitsstatus.</span><span class="sxs-lookup"><span data-stu-id="24494-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="24494-173">Mögliche Werte sind: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM` und `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="24494-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="24494-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="24494-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="24494-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="24494-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="24494-176">Virtualisierung-basierte Sicherheitsstatus.</span><span class="sxs-lookup"><span data-stu-id="24494-176">Virtualization-based security status.</span></span> <span data-ttu-id="24494-177">.</span><span class="sxs-lookup"><span data-stu-id="24494-177"></span></span> <span data-ttu-id="24494-178">Mögliche Werte sind: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements` und `other`.</span><span class="sxs-lookup"><span data-stu-id="24494-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="24494-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="24494-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="24494-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="24494-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="24494-181">Lokales System Autorität (LSA) Anmeldeinformationen Guard Status.</span><span class="sxs-lookup"><span data-stu-id="24494-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="24494-182">.</span><span class="sxs-lookup"><span data-stu-id="24494-182"></span></span> <span data-ttu-id="24494-183">Mögliche Werte sind: `running`, `rebootRequired`, `notLicensed`, `notConfigured` und `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="24494-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24494-184">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="24494-184">Relationships</span></span>
<span data-ttu-id="24494-185">Keine</span><span class="sxs-lookup"><span data-stu-id="24494-185">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24494-186">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="24494-186">JSON Representation</span></span>
<span data-ttu-id="24494-187">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="24494-187">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





