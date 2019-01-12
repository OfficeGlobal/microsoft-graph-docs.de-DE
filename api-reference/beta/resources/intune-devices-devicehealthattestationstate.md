---
title: Ressourcentyp „deviceHealthAttestationState“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03729d2c3a3f61c74bf7966f67a12084b7d24e25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987873"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="3cfcb-103">Ressourcentyp „deviceHealthAttestationState“</span><span class="sxs-lookup"><span data-stu-id="3cfcb-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="3cfcb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cfcb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cfcb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cfcb-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3cfcb-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3cfcb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3cfcb-108">Properties</span></span>
|<span data-ttu-id="3cfcb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3cfcb-109">Property</span></span>|<span data-ttu-id="3cfcb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3cfcb-110">Type</span></span>|<span data-ttu-id="3cfcb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cfcb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cfcb-112">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="3cfcb-112">lastUpdateDateTime</span></span>|<span data-ttu-id="3cfcb-113">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-113">String</span></span>|<span data-ttu-id="3cfcb-114">Zeitstempel der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="3cfcb-114">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="3cfcb-115">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="3cfcb-115">contentNamespaceUrl</span></span>|<span data-ttu-id="3cfcb-116">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-116">String</span></span>|<span data-ttu-id="3cfcb-117">Version des DHA-Berichts</span><span class="sxs-lookup"><span data-stu-id="3cfcb-117">The DHA report version.</span></span> <span data-ttu-id="3cfcb-118">(Version des Namespace)</span><span class="sxs-lookup"><span data-stu-id="3cfcb-118">(Namespace version)</span></span>|
|<span data-ttu-id="3cfcb-119">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="3cfcb-119">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="3cfcb-120">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-120">String</span></span>|<span data-ttu-id="3cfcb-121">Version des DHA-Berichts</span><span class="sxs-lookup"><span data-stu-id="3cfcb-121">The DHA report version.</span></span> <span data-ttu-id="3cfcb-122">(Version des Namespace)</span><span class="sxs-lookup"><span data-stu-id="3cfcb-122">(Namespace version)</span></span>|
|<span data-ttu-id="3cfcb-123">contentVersion</span><span class="sxs-lookup"><span data-stu-id="3cfcb-123">contentVersion</span></span>|<span data-ttu-id="3cfcb-124">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-124">String</span></span>|<span data-ttu-id="3cfcb-125">Version des Integritätsnachweisstatus-Schemas</span><span class="sxs-lookup"><span data-stu-id="3cfcb-125">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="3cfcb-126">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cfcb-126">issuedDateTime</span></span>|<span data-ttu-id="3cfcb-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cfcb-127">DateTimeOffset</span></span>|<span data-ttu-id="3cfcb-128">Datum und Uhrzeit der Evaluierung des Geräts durch eine MDM-Lösung bzw. der Registrierung des Geräts in einer MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="3cfcb-128">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="3cfcb-129">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="3cfcb-129">attestationIdentityKey</span></span>|<span data-ttu-id="3cfcb-130">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-130">String</span></span>|<span data-ttu-id="3cfcb-131">Ist auf einem Gerät ein AIK (Attestation Identity Key) vorhanden, bedeutet das, dass das Gerät über ein EK-Zertifikat (Endorsement Key-Zertifikat) verfügt.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-131">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="3cfcb-132">resetCount</span><span class="sxs-lookup"><span data-stu-id="3cfcb-132">resetCount</span></span>|<span data-ttu-id="3cfcb-133">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfcb-133">Int64</span></span>|<span data-ttu-id="3cfcb-134">Häufigkeit, mit der ein PC-Gerät in den Ruhezustand gewechselt bzw. den Betrieb fortgesetzt hat</span><span class="sxs-lookup"><span data-stu-id="3cfcb-134">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="3cfcb-135">restartCount</span><span class="sxs-lookup"><span data-stu-id="3cfcb-135">restartCount</span></span>|<span data-ttu-id="3cfcb-136">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfcb-136">Int64</span></span>|<span data-ttu-id="3cfcb-137">Häufigkeit, mit der ein PC-Gerät neu gestartet wurde</span><span class="sxs-lookup"><span data-stu-id="3cfcb-137">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="3cfcb-138">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="3cfcb-138">dataExcutionPolicy</span></span>|<span data-ttu-id="3cfcb-139">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-139">String</span></span>|<span data-ttu-id="3cfcb-140">Eine DEP-Richtlinie definiert eine Reihe von Hardware- und Softwaretechnologien, die zusätzliche Arbeitsspeicherprüfungen durchführen.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-140">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="3cfcb-141">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="3cfcb-141">bitLockerStatus</span></span>|<span data-ttu-id="3cfcb-142">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-142">String</span></span>|<span data-ttu-id="3cfcb-143">Aktiviert oder deaktiviert die BitLocker-Laufwerkverschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-143">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="3cfcb-144">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="3cfcb-144">bootManagerVersion</span></span>|<span data-ttu-id="3cfcb-145">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-145">String</span></span>|<span data-ttu-id="3cfcb-146">Version des Start-Managers</span><span class="sxs-lookup"><span data-stu-id="3cfcb-146">The version of the Boot Manager</span></span>|
|<span data-ttu-id="3cfcb-147">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="3cfcb-147">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="3cfcb-148">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-148">String</span></span>|<span data-ttu-id="3cfcb-149">Version des Start-Managers</span><span class="sxs-lookup"><span data-stu-id="3cfcb-149">The version of the Boot Manager</span></span>|
|<span data-ttu-id="3cfcb-150">secureBoot</span><span class="sxs-lookup"><span data-stu-id="3cfcb-150">secureBoot</span></span>|<span data-ttu-id="3cfcb-151">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-151">String</span></span>|<span data-ttu-id="3cfcb-152">Ist „secureBoot“ aktiviert, müssen die Hauptkomponenten über die korrekten Kryptografiesignaturen verfügen.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-152">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="3cfcb-153">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="3cfcb-153">bootDebugging</span></span>|<span data-ttu-id="3cfcb-154">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-154">String</span></span>|<span data-ttu-id="3cfcb-155">Ist „bootDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-155">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="3cfcb-156">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="3cfcb-156">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="3cfcb-157">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-157">String</span></span>|<span data-ttu-id="3cfcb-158">Ist „operatingSystemKernelDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-158">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="3cfcb-159">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="3cfcb-159">codeIntegrity</span></span>|<span data-ttu-id="3cfcb-160">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-160">String</span></span>| <span data-ttu-id="3cfcb-161">Ist „codeIntegrity“ aktiviert, wird ausschließlich Code ausgeführt, dessen Integrität verifiziert wurde.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-161">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="3cfcb-162">testSigning</span><span class="sxs-lookup"><span data-stu-id="3cfcb-162">testSigning</span></span>|<span data-ttu-id="3cfcb-163">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-163">String</span></span>|<span data-ttu-id="3cfcb-164">Ist „testSigning“ aktiviert, wird vom Gerät während des Starts keine Signaturprüfung erzwungen.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-164">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="3cfcb-165">safeMode</span><span class="sxs-lookup"><span data-stu-id="3cfcb-165">safeMode</span></span>|<span data-ttu-id="3cfcb-166">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-166">String</span></span>|<span data-ttu-id="3cfcb-167">Der abgesicherte Modus ist eine Option zur Problembehandlung unter Windows. Sie startet den Computer in einen eingeschränkten Zustand.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-167">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="3cfcb-168">windowsPE</span><span class="sxs-lookup"><span data-stu-id="3cfcb-168">windowsPE</span></span>|<span data-ttu-id="3cfcb-169">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-169">String</span></span>|<span data-ttu-id="3cfcb-170">Betriebssystem mit eingeschränkten Diensten, das den Computer für Windows vorbereitet</span><span class="sxs-lookup"><span data-stu-id="3cfcb-170">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="3cfcb-171">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="3cfcb-171">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="3cfcb-172">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-172">String</span></span>|<span data-ttu-id="3cfcb-173">ELAM schützt die Computer in Ihrem Netzwerk, während sie starten.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-173">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="3cfcb-174">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="3cfcb-174">virtualSecureMode</span></span>|<span data-ttu-id="3cfcb-175">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-175">String</span></span>|<span data-ttu-id="3cfcb-176">VSM ist ein Container, der bei Kernelkompromittierung wichtige Komponenten schützt.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-176">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="3cfcb-177">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3cfcb-177">pcrHashAlgorithm</span></span>|<span data-ttu-id="3cfcb-178">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-178">String</span></span>|<span data-ttu-id="3cfcb-179">Informationsattribut, das den Hashalgorithmus angibt, der vom TPM verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="3cfcb-179">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="3cfcb-180">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="3cfcb-180">bootAppSecurityVersion</span></span>|<span data-ttu-id="3cfcb-181">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-181">String</span></span>|<span data-ttu-id="3cfcb-182">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="3cfcb-182">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="3cfcb-183">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="3cfcb-183">bootManagerSecurityVersion</span></span>|<span data-ttu-id="3cfcb-184">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-184">String</span></span>|<span data-ttu-id="3cfcb-185">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="3cfcb-185">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="3cfcb-186">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="3cfcb-186">tpmVersion</span></span>|<span data-ttu-id="3cfcb-187">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-187">String</span></span>|<span data-ttu-id="3cfcb-188">Sicherheitsversionsnummer der Startanwendung</span><span class="sxs-lookup"><span data-stu-id="3cfcb-188">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="3cfcb-189">pcr0</span><span class="sxs-lookup"><span data-stu-id="3cfcb-189">pcr0</span></span>|<span data-ttu-id="3cfcb-190">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-190">String</span></span>|<span data-ttu-id="3cfcb-191">Kennzahl, die in PCR\[0\] erfasst ist</span><span class="sxs-lookup"><span data-stu-id="3cfcb-191">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="3cfcb-192">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="3cfcb-192">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="3cfcb-193">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-193">String</span></span>|<span data-ttu-id="3cfcb-194">Fingerabdruck der benutzerdefinierten Richtlinie für die Konfiguration der Option „Sicherer Start“</span><span class="sxs-lookup"><span data-stu-id="3cfcb-194">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="3cfcb-195">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="3cfcb-195">codeIntegrityPolicy</span></span>|<span data-ttu-id="3cfcb-196">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-196">String</span></span>|<span data-ttu-id="3cfcb-197">Die Codeintegritätsrichtlinie, die die Sicherheit der Startumgebung steuert</span><span class="sxs-lookup"><span data-stu-id="3cfcb-197">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="3cfcb-198">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="3cfcb-198">bootRevisionListInfo</span></span>|<span data-ttu-id="3cfcb-199">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-199">String</span></span>|<span data-ttu-id="3cfcb-200">Die Startüberarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde</span><span class="sxs-lookup"><span data-stu-id="3cfcb-200">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="3cfcb-201">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="3cfcb-201">operatingSystemRevListInfo</span></span>|<span data-ttu-id="3cfcb-202">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-202">String</span></span>|<span data-ttu-id="3cfcb-203">Die Betriebssystem-Überarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde</span><span class="sxs-lookup"><span data-stu-id="3cfcb-203">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="3cfcb-204">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="3cfcb-204">healthStatusMismatchInfo</span></span>|<span data-ttu-id="3cfcb-205">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-205">String</span></span>|<span data-ttu-id="3cfcb-206">Dieses Attribut wird angezeigt, wenn der DHA-Dienst ein Integritätsproblem erkennt.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-206">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="3cfcb-207">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="3cfcb-207">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="3cfcb-208">String</span><span class="sxs-lookup"><span data-stu-id="3cfcb-208">String</span></span>|<span data-ttu-id="3cfcb-209">Dieses Attribut gibt an, ob das Gerät DHA unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-209">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cfcb-210">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3cfcb-210">Relationships</span></span>
<span data-ttu-id="3cfcb-211">Keine</span><span class="sxs-lookup"><span data-stu-id="3cfcb-211">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3cfcb-212">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3cfcb-212">JSON Representation</span></span>
<span data-ttu-id="3cfcb-213">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3cfcb-213">Here is a JSON representation of the resource.</span></span>
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





