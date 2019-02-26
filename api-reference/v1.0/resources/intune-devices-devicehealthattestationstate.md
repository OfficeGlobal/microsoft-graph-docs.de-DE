---
title: Ressourcentyp „deviceHealthAttestationState“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53fa5cdafdc125fdc32ef599a625c58e3bcbe687
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256147"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="579f8-103">Ressourcentyp „deviceHealthAttestationState“</span><span class="sxs-lookup"><span data-stu-id="579f8-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="579f8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="579f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="579f8-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="579f8-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="579f8-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="579f8-106">Properties</span></span>
|<span data-ttu-id="579f8-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="579f8-107">Property</span></span>|<span data-ttu-id="579f8-108">Typ</span><span class="sxs-lookup"><span data-stu-id="579f8-108">Type</span></span>|<span data-ttu-id="579f8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="579f8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="579f8-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="579f8-110">lastUpdateDateTime</span></span>|<span data-ttu-id="579f8-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-111">String</span></span>|<span data-ttu-id="579f8-112">Zeitstempel der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="579f8-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="579f8-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="579f8-113">contentNamespaceUrl</span></span>|<span data-ttu-id="579f8-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-114">String</span></span>|<span data-ttu-id="579f8-115">Version des DHA-Berichts</span><span class="sxs-lookup"><span data-stu-id="579f8-115">The DHA report version.</span></span> <span data-ttu-id="579f8-116">(Version des Namespace)</span><span class="sxs-lookup"><span data-stu-id="579f8-116">(Namespace version)</span></span>|
|<span data-ttu-id="579f8-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="579f8-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="579f8-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-118">String</span></span>|<span data-ttu-id="579f8-119">Version des DHA-Berichts</span><span class="sxs-lookup"><span data-stu-id="579f8-119">The DHA report version.</span></span> <span data-ttu-id="579f8-120">(Version des Namespace)</span><span class="sxs-lookup"><span data-stu-id="579f8-120">(Namespace version)</span></span>|
|<span data-ttu-id="579f8-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="579f8-121">contentVersion</span></span>|<span data-ttu-id="579f8-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-122">String</span></span>|<span data-ttu-id="579f8-123">Version des Integritätsnachweisstatus-Schemas</span><span class="sxs-lookup"><span data-stu-id="579f8-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="579f8-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="579f8-124">issuedDateTime</span></span>|<span data-ttu-id="579f8-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="579f8-125">DateTimeOffset</span></span>|<span data-ttu-id="579f8-126">Datum und Uhrzeit der Evaluierung des Geräts durch eine MDM-Lösung bzw. der Registrierung des Geräts in einer MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="579f8-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="579f8-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="579f8-127">attestationIdentityKey</span></span>|<span data-ttu-id="579f8-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-128">String</span></span>|<span data-ttu-id="579f8-129">Ist auf einem Gerät ein AIK (Attestation Identity Key) vorhanden, bedeutet das, dass das Gerät über ein EK-Zertifikat (Endorsement Key-Zertifikat) verfügt.</span><span class="sxs-lookup"><span data-stu-id="579f8-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="579f8-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="579f8-130">resetCount</span></span>|<span data-ttu-id="579f8-131">Int64</span><span class="sxs-lookup"><span data-stu-id="579f8-131">Int64</span></span>|<span data-ttu-id="579f8-132">Häufigkeit, mit der ein PC-Gerät in den Ruhezustand gewechselt bzw. den Betrieb fortgesetzt hat</span><span class="sxs-lookup"><span data-stu-id="579f8-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="579f8-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="579f8-133">restartCount</span></span>|<span data-ttu-id="579f8-134">Int64</span><span class="sxs-lookup"><span data-stu-id="579f8-134">Int64</span></span>|<span data-ttu-id="579f8-135">Häufigkeit, mit der ein PC-Gerät neu gestartet wurde</span><span class="sxs-lookup"><span data-stu-id="579f8-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="579f8-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="579f8-136">dataExcutionPolicy</span></span>|<span data-ttu-id="579f8-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-137">String</span></span>|<span data-ttu-id="579f8-138">Eine DEP-Richtlinie definiert eine Reihe von Hardware- und Softwaretechnologien, die zusätzliche Arbeitsspeicherprüfungen durchführen.</span><span class="sxs-lookup"><span data-stu-id="579f8-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="579f8-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="579f8-139">bitLockerStatus</span></span>|<span data-ttu-id="579f8-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-140">String</span></span>|<span data-ttu-id="579f8-141">Aktiviert oder deaktiviert die BitLocker-Laufwerkverschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="579f8-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="579f8-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="579f8-142">bootManagerVersion</span></span>|<span data-ttu-id="579f8-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-143">String</span></span>|<span data-ttu-id="579f8-144">Version des Start-Managers</span><span class="sxs-lookup"><span data-stu-id="579f8-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="579f8-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="579f8-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="579f8-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-146">String</span></span>|<span data-ttu-id="579f8-147">Version des Start-Managers</span><span class="sxs-lookup"><span data-stu-id="579f8-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="579f8-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="579f8-148">secureBoot</span></span>|<span data-ttu-id="579f8-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-149">String</span></span>|<span data-ttu-id="579f8-150">Ist „secureBoot“ aktiviert, müssen die Hauptkomponenten über die korrekten Kryptografiesignaturen verfügen.</span><span class="sxs-lookup"><span data-stu-id="579f8-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="579f8-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="579f8-151">bootDebugging</span></span>|<span data-ttu-id="579f8-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-152">String</span></span>|<span data-ttu-id="579f8-153">Ist „bootDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.</span><span class="sxs-lookup"><span data-stu-id="579f8-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="579f8-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="579f8-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="579f8-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-155">String</span></span>|<span data-ttu-id="579f8-156">Ist „operatingSystemKernelDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.</span><span class="sxs-lookup"><span data-stu-id="579f8-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="579f8-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="579f8-157">codeIntegrity</span></span>|<span data-ttu-id="579f8-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-158">String</span></span>| <span data-ttu-id="579f8-159">Ist „codeIntegrity“ aktiviert, wird ausschließlich Code ausgeführt, dessen Integrität verifiziert wurde.</span><span class="sxs-lookup"><span data-stu-id="579f8-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="579f8-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="579f8-160">testSigning</span></span>|<span data-ttu-id="579f8-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-161">String</span></span>|<span data-ttu-id="579f8-162">Ist „testSigning“ aktiviert, wird vom Gerät während des Starts keine Signaturprüfung erzwungen.</span><span class="sxs-lookup"><span data-stu-id="579f8-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="579f8-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="579f8-163">safeMode</span></span>|<span data-ttu-id="579f8-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-164">String</span></span>|<span data-ttu-id="579f8-165">Der abgesicherte Modus ist eine Option zur Problembehandlung unter Windows. Sie startet den Computer in einen eingeschränkten Zustand.</span><span class="sxs-lookup"><span data-stu-id="579f8-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="579f8-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="579f8-166">windowsPE</span></span>|<span data-ttu-id="579f8-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-167">String</span></span>|<span data-ttu-id="579f8-168">Betriebssystem mit eingeschränkten Diensten, das den Computer für Windows vorbereitet</span><span class="sxs-lookup"><span data-stu-id="579f8-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="579f8-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="579f8-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="579f8-170">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-170">String</span></span>|<span data-ttu-id="579f8-171">ELAM schützt die Computer in Ihrem Netzwerk, während sie starten.</span><span class="sxs-lookup"><span data-stu-id="579f8-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="579f8-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="579f8-172">virtualSecureMode</span></span>|<span data-ttu-id="579f8-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-173">String</span></span>|<span data-ttu-id="579f8-174">VSM ist ein Container, der bei Kernelkompromittierung wichtige Komponenten schützt.</span><span class="sxs-lookup"><span data-stu-id="579f8-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="579f8-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="579f8-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="579f8-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-176">String</span></span>|<span data-ttu-id="579f8-177">Informationsattribut, das den Hashalgorithmus angibt, der vom TPM verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="579f8-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="579f8-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="579f8-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="579f8-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-179">String</span></span>|<span data-ttu-id="579f8-180">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="579f8-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="579f8-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="579f8-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="579f8-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-182">String</span></span>|<span data-ttu-id="579f8-183">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="579f8-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="579f8-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="579f8-184">tpmVersion</span></span>|<span data-ttu-id="579f8-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-185">String</span></span>|<span data-ttu-id="579f8-186">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="579f8-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="579f8-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="579f8-187">pcr0</span></span>|<span data-ttu-id="579f8-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-188">String</span></span>|<span data-ttu-id="579f8-189">Kennzahl, die in PCR\[0\] erfasst ist</span><span class="sxs-lookup"><span data-stu-id="579f8-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="579f8-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="579f8-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="579f8-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-191">String</span></span>|<span data-ttu-id="579f8-192">Fingerabdruck der benutzerdefinierten Richtlinie für die Konfiguration der Option „Sicherer Start“</span><span class="sxs-lookup"><span data-stu-id="579f8-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="579f8-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="579f8-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="579f8-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-194">String</span></span>|<span data-ttu-id="579f8-195">Die Codeintegritätsrichtlinie, die die Sicherheit der Startumgebung steuert</span><span class="sxs-lookup"><span data-stu-id="579f8-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="579f8-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="579f8-196">bootRevisionListInfo</span></span>|<span data-ttu-id="579f8-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-197">String</span></span>|<span data-ttu-id="579f8-198">Die Startüberarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde</span><span class="sxs-lookup"><span data-stu-id="579f8-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="579f8-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="579f8-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="579f8-200">String</span><span class="sxs-lookup"><span data-stu-id="579f8-200">String</span></span>|<span data-ttu-id="579f8-201">Die Betriebssystem-Überarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde</span><span class="sxs-lookup"><span data-stu-id="579f8-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="579f8-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="579f8-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="579f8-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="579f8-203">String</span></span>|<span data-ttu-id="579f8-204">Dieses Attribut wird angezeigt, wenn der DHA-Dienst ein Integritätsproblem erkennt.</span><span class="sxs-lookup"><span data-stu-id="579f8-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="579f8-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="579f8-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="579f8-206">String</span><span class="sxs-lookup"><span data-stu-id="579f8-206">String</span></span>|<span data-ttu-id="579f8-207">Dieses Attribut gibt an, ob das Gerät DHA unterstützt.</span><span class="sxs-lookup"><span data-stu-id="579f8-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="579f8-208">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="579f8-208">Relationships</span></span>
<span data-ttu-id="579f8-209">Keine</span><span class="sxs-lookup"><span data-stu-id="579f8-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="579f8-210">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="579f8-210">JSON Representation</span></span>
<span data-ttu-id="579f8-211">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="579f8-211">Here is a JSON representation of the resource.</span></span>
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



