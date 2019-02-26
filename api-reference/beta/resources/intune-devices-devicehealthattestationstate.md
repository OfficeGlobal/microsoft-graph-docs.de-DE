---
title: Ressourcentyp „deviceHealthAttestationState“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca4e5f1da8dc03c98c3d5e72fc03177cdcbf38b2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157463"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="ab68a-103">Ressourcentyp „deviceHealthAttestationState“</span><span class="sxs-lookup"><span data-stu-id="ab68a-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="ab68a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ab68a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab68a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ab68a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab68a-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ab68a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ab68a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ab68a-107">Properties</span></span>
|<span data-ttu-id="ab68a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab68a-108">Property</span></span>|<span data-ttu-id="ab68a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ab68a-109">Type</span></span>|<span data-ttu-id="ab68a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab68a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab68a-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ab68a-111">lastUpdateDateTime</span></span>|<span data-ttu-id="ab68a-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-112">String</span></span>|<span data-ttu-id="ab68a-113">Zeitstempel der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="ab68a-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="ab68a-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="ab68a-114">contentNamespaceUrl</span></span>|<span data-ttu-id="ab68a-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-115">String</span></span>|<span data-ttu-id="ab68a-116">Version des DHA-Berichts</span><span class="sxs-lookup"><span data-stu-id="ab68a-116">The DHA report version.</span></span> <span data-ttu-id="ab68a-117">(Version des Namespace)</span><span class="sxs-lookup"><span data-stu-id="ab68a-117">(Namespace version)</span></span>|
|<span data-ttu-id="ab68a-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="ab68a-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="ab68a-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-119">String</span></span>|<span data-ttu-id="ab68a-120">Version des DHA-Berichts</span><span class="sxs-lookup"><span data-stu-id="ab68a-120">The DHA report version.</span></span> <span data-ttu-id="ab68a-121">(Version des Namespace)</span><span class="sxs-lookup"><span data-stu-id="ab68a-121">(Namespace version)</span></span>|
|<span data-ttu-id="ab68a-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="ab68a-122">contentVersion</span></span>|<span data-ttu-id="ab68a-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-123">String</span></span>|<span data-ttu-id="ab68a-124">Version des Integritätsnachweisstatus-Schemas</span><span class="sxs-lookup"><span data-stu-id="ab68a-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="ab68a-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab68a-125">issuedDateTime</span></span>|<span data-ttu-id="ab68a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab68a-126">DateTimeOffset</span></span>|<span data-ttu-id="ab68a-127">Datum und Uhrzeit der Evaluierung des Geräts durch eine MDM-Lösung bzw. der Registrierung des Geräts in einer MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="ab68a-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="ab68a-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="ab68a-128">attestationIdentityKey</span></span>|<span data-ttu-id="ab68a-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-129">String</span></span>|<span data-ttu-id="ab68a-130">Ist auf einem Gerät ein AIK (Attestation Identity Key) vorhanden, bedeutet das, dass das Gerät über ein EK-Zertifikat (Endorsement Key-Zertifikat) verfügt.</span><span class="sxs-lookup"><span data-stu-id="ab68a-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="ab68a-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="ab68a-131">resetCount</span></span>|<span data-ttu-id="ab68a-132">Int64</span><span class="sxs-lookup"><span data-stu-id="ab68a-132">Int64</span></span>|<span data-ttu-id="ab68a-133">Häufigkeit, mit der ein PC-Gerät in den Ruhezustand gewechselt bzw. den Betrieb fortgesetzt hat</span><span class="sxs-lookup"><span data-stu-id="ab68a-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="ab68a-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="ab68a-134">restartCount</span></span>|<span data-ttu-id="ab68a-135">Int64</span><span class="sxs-lookup"><span data-stu-id="ab68a-135">Int64</span></span>|<span data-ttu-id="ab68a-136">Häufigkeit, mit der ein PC-Gerät neu gestartet wurde</span><span class="sxs-lookup"><span data-stu-id="ab68a-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="ab68a-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="ab68a-137">dataExcutionPolicy</span></span>|<span data-ttu-id="ab68a-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-138">String</span></span>|<span data-ttu-id="ab68a-139">Eine DEP-Richtlinie definiert eine Reihe von Hardware- und Softwaretechnologien, die zusätzliche Arbeitsspeicherprüfungen durchführen.</span><span class="sxs-lookup"><span data-stu-id="ab68a-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="ab68a-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="ab68a-140">bitLockerStatus</span></span>|<span data-ttu-id="ab68a-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-141">String</span></span>|<span data-ttu-id="ab68a-142">Aktiviert oder deaktiviert die BitLocker-Laufwerkverschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="ab68a-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="ab68a-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="ab68a-143">bootManagerVersion</span></span>|<span data-ttu-id="ab68a-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-144">String</span></span>|<span data-ttu-id="ab68a-145">Version des Start-Managers</span><span class="sxs-lookup"><span data-stu-id="ab68a-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="ab68a-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="ab68a-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="ab68a-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-147">String</span></span>|<span data-ttu-id="ab68a-148">Version des Start-Managers</span><span class="sxs-lookup"><span data-stu-id="ab68a-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="ab68a-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="ab68a-149">secureBoot</span></span>|<span data-ttu-id="ab68a-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-150">String</span></span>|<span data-ttu-id="ab68a-151">Ist „secureBoot“ aktiviert, müssen die Hauptkomponenten über die korrekten Kryptografiesignaturen verfügen.</span><span class="sxs-lookup"><span data-stu-id="ab68a-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="ab68a-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="ab68a-152">bootDebugging</span></span>|<span data-ttu-id="ab68a-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-153">String</span></span>|<span data-ttu-id="ab68a-154">Ist „bootDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.</span><span class="sxs-lookup"><span data-stu-id="ab68a-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="ab68a-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="ab68a-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="ab68a-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-156">String</span></span>|<span data-ttu-id="ab68a-157">Ist „operatingSystemKernelDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.</span><span class="sxs-lookup"><span data-stu-id="ab68a-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="ab68a-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="ab68a-158">codeIntegrity</span></span>|<span data-ttu-id="ab68a-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-159">String</span></span>| <span data-ttu-id="ab68a-160">Ist „codeIntegrity“ aktiviert, wird ausschließlich Code ausgeführt, dessen Integrität verifiziert wurde.</span><span class="sxs-lookup"><span data-stu-id="ab68a-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="ab68a-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="ab68a-161">testSigning</span></span>|<span data-ttu-id="ab68a-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-162">String</span></span>|<span data-ttu-id="ab68a-163">Ist „testSigning“ aktiviert, wird vom Gerät während des Starts keine Signaturprüfung erzwungen.</span><span class="sxs-lookup"><span data-stu-id="ab68a-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="ab68a-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="ab68a-164">safeMode</span></span>|<span data-ttu-id="ab68a-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-165">String</span></span>|<span data-ttu-id="ab68a-166">Der abgesicherte Modus ist eine Option zur Problembehandlung unter Windows. Sie startet den Computer in einen eingeschränkten Zustand.</span><span class="sxs-lookup"><span data-stu-id="ab68a-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="ab68a-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="ab68a-167">windowsPE</span></span>|<span data-ttu-id="ab68a-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-168">String</span></span>|<span data-ttu-id="ab68a-169">Betriebssystem mit eingeschränkten Diensten, das den Computer für Windows vorbereitet</span><span class="sxs-lookup"><span data-stu-id="ab68a-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="ab68a-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="ab68a-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="ab68a-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-171">String</span></span>|<span data-ttu-id="ab68a-172">ELAM schützt die Computer in Ihrem Netzwerk, während sie starten.</span><span class="sxs-lookup"><span data-stu-id="ab68a-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="ab68a-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="ab68a-173">virtualSecureMode</span></span>|<span data-ttu-id="ab68a-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-174">String</span></span>|<span data-ttu-id="ab68a-175">VSM ist ein Container, der bei Kernelkompromittierung wichtige Komponenten schützt.</span><span class="sxs-lookup"><span data-stu-id="ab68a-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="ab68a-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ab68a-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="ab68a-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-177">String</span></span>|<span data-ttu-id="ab68a-178">Informationsattribut, das den Hashalgorithmus angibt, der vom TPM verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="ab68a-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="ab68a-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="ab68a-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="ab68a-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-180">String</span></span>|<span data-ttu-id="ab68a-181">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="ab68a-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="ab68a-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="ab68a-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="ab68a-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-183">String</span></span>|<span data-ttu-id="ab68a-184">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="ab68a-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="ab68a-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="ab68a-185">tpmVersion</span></span>|<span data-ttu-id="ab68a-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-186">String</span></span>|<span data-ttu-id="ab68a-187">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="ab68a-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="ab68a-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="ab68a-188">pcr0</span></span>|<span data-ttu-id="ab68a-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-189">String</span></span>|<span data-ttu-id="ab68a-190">Kennzahl, die in PCR\[0\] erfasst ist</span><span class="sxs-lookup"><span data-stu-id="ab68a-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="ab68a-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="ab68a-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="ab68a-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-192">String</span></span>|<span data-ttu-id="ab68a-193">Fingerabdruck der benutzerdefinierten Richtlinie für die Konfiguration der Option „Sicherer Start“</span><span class="sxs-lookup"><span data-stu-id="ab68a-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="ab68a-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="ab68a-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="ab68a-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-195">String</span></span>|<span data-ttu-id="ab68a-196">Die Codeintegritätsrichtlinie, die die Sicherheit der Startumgebung steuert</span><span class="sxs-lookup"><span data-stu-id="ab68a-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="ab68a-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="ab68a-197">bootRevisionListInfo</span></span>|<span data-ttu-id="ab68a-198">String</span><span class="sxs-lookup"><span data-stu-id="ab68a-198">String</span></span>|<span data-ttu-id="ab68a-199">Die Startüberarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde</span><span class="sxs-lookup"><span data-stu-id="ab68a-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="ab68a-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="ab68a-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="ab68a-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-201">String</span></span>|<span data-ttu-id="ab68a-202">Die Betriebssystem-Überarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde</span><span class="sxs-lookup"><span data-stu-id="ab68a-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="ab68a-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="ab68a-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="ab68a-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab68a-204">String</span></span>|<span data-ttu-id="ab68a-205">Dieses Attribut wird angezeigt, wenn der DHA-Dienst ein Integritätsproblem erkennt.</span><span class="sxs-lookup"><span data-stu-id="ab68a-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="ab68a-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="ab68a-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="ab68a-207">String</span><span class="sxs-lookup"><span data-stu-id="ab68a-207">String</span></span>|<span data-ttu-id="ab68a-208">Dieses Attribut gibt an, ob das Gerät DHA unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ab68a-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab68a-209">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ab68a-209">Relationships</span></span>
<span data-ttu-id="ab68a-210">Keine</span><span class="sxs-lookup"><span data-stu-id="ab68a-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab68a-211">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ab68a-211">JSON Representation</span></span>
<span data-ttu-id="ab68a-212">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ab68a-212">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```




