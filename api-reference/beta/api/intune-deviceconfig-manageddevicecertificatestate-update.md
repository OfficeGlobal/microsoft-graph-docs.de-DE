---
title: ManagedDeviceCertificateState aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ManagedDeviceCertificateState-Objekts.
author: tfitzmac
ms.openlocfilehash: 14c73bf219d8a568f8df0c4c55e3a1e3d0516abd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350169"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="cedbd-103">ManagedDeviceCertificateState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cedbd-103">Update managedDeviceCertificateState</span></span>

> <span data-ttu-id="cedbd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cedbd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cedbd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cedbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cedbd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cedbd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cedbd-107">Aktualisieren Sie die Eigenschaften eines [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cedbd-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cedbd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cedbd-108">Prerequisites</span></span>
<span data-ttu-id="cedbd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cedbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cedbd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cedbd-111">Permission type</span></span>|<span data-ttu-id="cedbd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cedbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cedbd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cedbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cedbd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cedbd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cedbd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cedbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cedbd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cedbd-116">Not supported.</span></span>|
|<span data-ttu-id="cedbd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cedbd-117">Application</span></span>|<span data-ttu-id="cedbd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cedbd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cedbd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cedbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="cedbd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cedbd-120">Request headers</span></span>
|<span data-ttu-id="cedbd-121">Header</span><span class="sxs-lookup"><span data-stu-id="cedbd-121">Header</span></span>|<span data-ttu-id="cedbd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cedbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cedbd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cedbd-123">Authorization</span></span>|<span data-ttu-id="cedbd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cedbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cedbd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cedbd-125">Accept</span></span>|<span data-ttu-id="cedbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cedbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cedbd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cedbd-127">Request body</span></span>
<span data-ttu-id="cedbd-128">Geben Sie im Textkörper Anforderung für das Objekt [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="cedbd-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="cedbd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="cedbd-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="cedbd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cedbd-130">Property</span></span>|<span data-ttu-id="cedbd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cedbd-131">Type</span></span>|<span data-ttu-id="cedbd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cedbd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cedbd-133">id</span><span class="sxs-lookup"><span data-stu-id="cedbd-133">id</span></span>|<span data-ttu-id="cedbd-134">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-134">String</span></span>|<span data-ttu-id="cedbd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cedbd-135">Key of the entity.</span></span>|
|<span data-ttu-id="cedbd-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="cedbd-136">devicePlatform</span></span>|[<span data-ttu-id="cedbd-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="cedbd-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="cedbd-138">Geräteplattform.</span><span class="sxs-lookup"><span data-stu-id="cedbd-138">Device platform.</span></span> <span data-ttu-id="cedbd-139">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="cedbd-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="cedbd-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="cedbd-140">certificateKeyUsage</span></span>|[<span data-ttu-id="cedbd-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="cedbd-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="cedbd-142">Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="cedbd-142">Key usage.</span></span> <span data-ttu-id="cedbd-143">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="cedbd-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="cedbd-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="cedbd-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="cedbd-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cedbd-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="cedbd-146">Gültigkeit Period Einheiten.</span><span class="sxs-lookup"><span data-stu-id="cedbd-146">Validity period units.</span></span> <span data-ttu-id="cedbd-147">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="cedbd-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="cedbd-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="cedbd-148">certificateIssuanceState</span></span>|[<span data-ttu-id="cedbd-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="cedbd-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="cedbd-150">Veröffentlichungslizenzen Zustand.</span><span class="sxs-lookup"><span data-stu-id="cedbd-150">Issuance State.</span></span> <span data-ttu-id="cedbd-151">Mögliche Werte sind: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="cedbd-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="cedbd-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="cedbd-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="cedbd-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="cedbd-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="cedbd-154">Wichtige Speicheranbieter.</span><span class="sxs-lookup"><span data-stu-id="cedbd-154">Key Storage Provider.</span></span> <span data-ttu-id="cedbd-155">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="cedbd-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="cedbd-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cedbd-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="cedbd-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cedbd-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="cedbd-158">Format des Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="cedbd-158">Subject name format.</span></span> <span data-ttu-id="cedbd-159">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="cedbd-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="cedbd-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="cedbd-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="cedbd-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cedbd-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="cedbd-162">Subject alternative Name-Format.</span><span class="sxs-lookup"><span data-stu-id="cedbd-162">Subject alternative name format.</span></span> <span data-ttu-id="cedbd-163">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="cedbd-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="cedbd-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="cedbd-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="cedbd-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="cedbd-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="cedbd-166">REVOKE-Status.</span><span class="sxs-lookup"><span data-stu-id="cedbd-166">Revoke status.</span></span> <span data-ttu-id="cedbd-167">Mögliche Werte sind: `none`, `pending`, `issued`, `failed` und `revoked`.</span><span class="sxs-lookup"><span data-stu-id="cedbd-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="cedbd-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="cedbd-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="cedbd-169">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-169">String</span></span>|<span data-ttu-id="cedbd-170">Profil der Anzeigename des Zertifikats</span><span class="sxs-lookup"><span data-stu-id="cedbd-170">Certificate profile display name</span></span>|
|<span data-ttu-id="cedbd-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cedbd-171">deviceDisplayName</span></span>|<span data-ttu-id="cedbd-172">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-172">String</span></span>|<span data-ttu-id="cedbd-173">Anzeigename des Geräts</span><span class="sxs-lookup"><span data-stu-id="cedbd-173">Device display name</span></span>|
|<span data-ttu-id="cedbd-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="cedbd-174">userDisplayName</span></span>|<span data-ttu-id="cedbd-175">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-175">String</span></span>|<span data-ttu-id="cedbd-176">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="cedbd-176">User display name</span></span>|
|<span data-ttu-id="cedbd-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cedbd-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="cedbd-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedbd-178">DateTimeOffset</span></span>|<span data-ttu-id="cedbd-179">Ablaufdatum des Zertifikats</span><span class="sxs-lookup"><span data-stu-id="cedbd-179">Certificate expiry date</span></span>|
|<span data-ttu-id="cedbd-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="cedbd-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="cedbd-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedbd-181">DateTimeOffset</span></span>|<span data-ttu-id="cedbd-182">Änderung des letzten Zertifikat Veröffentlichungslizenzen</span><span class="sxs-lookup"><span data-stu-id="cedbd-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="cedbd-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="cedbd-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="cedbd-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedbd-184">DateTimeOffset</span></span>|<span data-ttu-id="cedbd-185">Änderung des letzten Zertifikat Veröffentlichungslizenzen</span><span class="sxs-lookup"><span data-stu-id="cedbd-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="cedbd-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="cedbd-186">certificateIssuer</span></span>|<span data-ttu-id="cedbd-187">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-187">String</span></span>|<span data-ttu-id="cedbd-188">Aussteller</span><span class="sxs-lookup"><span data-stu-id="cedbd-188">Issuer</span></span>|
|<span data-ttu-id="cedbd-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="cedbd-189">certificateThumbprint</span></span>|<span data-ttu-id="cedbd-190">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-190">String</span></span>|<span data-ttu-id="cedbd-191">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="cedbd-191">Thumbprint</span></span>|
|<span data-ttu-id="cedbd-192">Zertifikatsseriennummer</span><span class="sxs-lookup"><span data-stu-id="cedbd-192">certificateSerialNumber</span></span>|<span data-ttu-id="cedbd-193">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-193">String</span></span>|<span data-ttu-id="cedbd-194">Seriennummer</span><span class="sxs-lookup"><span data-stu-id="cedbd-194">Serial number</span></span>|
|<span data-ttu-id="cedbd-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="cedbd-195">certificateKeyLength</span></span>|<span data-ttu-id="cedbd-196">Int32</span><span class="sxs-lookup"><span data-stu-id="cedbd-196">Int32</span></span>|<span data-ttu-id="cedbd-197">Schlüssellänge</span><span class="sxs-lookup"><span data-stu-id="cedbd-197">Key length</span></span>|
|<span data-ttu-id="cedbd-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="cedbd-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="cedbd-199">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-199">String</span></span>|<span data-ttu-id="cedbd-200">Erweiterte Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="cedbd-200">Extended key usage</span></span>|
|<span data-ttu-id="cedbd-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="cedbd-201">certificateValidityPeriod</span></span>|<span data-ttu-id="cedbd-202">Int32</span><span class="sxs-lookup"><span data-stu-id="cedbd-202">Int32</span></span>|<span data-ttu-id="cedbd-203">Gültigkeitsdauer</span><span class="sxs-lookup"><span data-stu-id="cedbd-203">Validity period</span></span>|
|<span data-ttu-id="cedbd-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="cedbd-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="cedbd-205">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-205">String</span></span>|<span data-ttu-id="cedbd-206">Subject Name Formatzeichenfolge für benutzerdefinierte Subject Namensformate</span><span class="sxs-lookup"><span data-stu-id="cedbd-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="cedbd-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="cedbd-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="cedbd-208">String</span><span class="sxs-lookup"><span data-stu-id="cedbd-208">String</span></span>|<span data-ttu-id="cedbd-209">Subject alternative Name Formatzeichenfolge für benutzerdefinierte Formate</span><span class="sxs-lookup"><span data-stu-id="cedbd-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="cedbd-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="cedbd-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="cedbd-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedbd-211">DateTimeOffset</span></span>|<span data-ttu-id="cedbd-212">Veröffentlichungslizenzen Datum</span><span class="sxs-lookup"><span data-stu-id="cedbd-212">Issuance date</span></span>|
|<span data-ttu-id="cedbd-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="cedbd-213">certificateErrorCode</span></span>|<span data-ttu-id="cedbd-214">Int32</span><span class="sxs-lookup"><span data-stu-id="cedbd-214">Int32</span></span>|<span data-ttu-id="cedbd-215">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="cedbd-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="cedbd-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="cedbd-216">Response</span></span>
<span data-ttu-id="cedbd-217">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cedbd-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cedbd-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cedbd-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="cedbd-219">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cedbd-219">Request</span></span>
<span data-ttu-id="cedbd-220">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cedbd-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
Content-type: application/json
Content-length: 1449

{
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```

### <a name="response"></a><span data-ttu-id="cedbd-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="cedbd-221">Response</span></span>
<span data-ttu-id="cedbd-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cedbd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1566

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```





