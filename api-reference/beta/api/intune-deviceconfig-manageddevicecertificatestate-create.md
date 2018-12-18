---
title: Erstellen von managedDeviceCertificateState
description: Erstellen eines neuen ManagedDeviceCertificateState-Objekts.
author: tfitzmac
ms.openlocfilehash: 22b8a0db82e86b9136ee997a821223afe608b51a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305957"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="d44ac-103">Erstellen von managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="d44ac-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="d44ac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d44ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d44ac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d44ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d44ac-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d44ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d44ac-107">Erstellen eines neuen [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d44ac-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d44ac-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d44ac-108">Prerequisites</span></span>
<span data-ttu-id="d44ac-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d44ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d44ac-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d44ac-111">Permission type</span></span>|<span data-ttu-id="d44ac-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d44ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d44ac-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d44ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d44ac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d44ac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d44ac-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d44ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d44ac-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d44ac-116">Not supported.</span></span>|
|<span data-ttu-id="d44ac-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d44ac-117">Application</span></span>|<span data-ttu-id="d44ac-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d44ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d44ac-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d44ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="d44ac-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d44ac-120">Request headers</span></span>
|<span data-ttu-id="d44ac-121">Header</span><span class="sxs-lookup"><span data-stu-id="d44ac-121">Header</span></span>|<span data-ttu-id="d44ac-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d44ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d44ac-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d44ac-123">Authorization</span></span>|<span data-ttu-id="d44ac-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d44ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d44ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d44ac-125">Accept</span></span>|<span data-ttu-id="d44ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d44ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d44ac-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d44ac-127">Request body</span></span>
<span data-ttu-id="d44ac-128">Geben Sie im Textkörper Anforderung für das Objekt ManagedDeviceCertificateState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d44ac-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="d44ac-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ManagedDeviceCertificateState erstellen.</span><span class="sxs-lookup"><span data-stu-id="d44ac-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="d44ac-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d44ac-130">Property</span></span>|<span data-ttu-id="d44ac-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d44ac-131">Type</span></span>|<span data-ttu-id="d44ac-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d44ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d44ac-133">id</span><span class="sxs-lookup"><span data-stu-id="d44ac-133">id</span></span>|<span data-ttu-id="d44ac-134">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-134">String</span></span>|<span data-ttu-id="d44ac-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d44ac-135">Key of the entity.</span></span>|
|<span data-ttu-id="d44ac-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="d44ac-136">devicePlatform</span></span>|[<span data-ttu-id="d44ac-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="d44ac-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="d44ac-138">Geräteplattform.</span><span class="sxs-lookup"><span data-stu-id="d44ac-138">Device platform.</span></span> <span data-ttu-id="d44ac-139">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="d44ac-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="d44ac-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="d44ac-140">certificateKeyUsage</span></span>|[<span data-ttu-id="d44ac-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="d44ac-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="d44ac-142">Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="d44ac-142">Key usage.</span></span> <span data-ttu-id="d44ac-143">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="d44ac-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="d44ac-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="d44ac-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="d44ac-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d44ac-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d44ac-146">Gültigkeit Period Einheiten.</span><span class="sxs-lookup"><span data-stu-id="d44ac-146">Validity period units.</span></span> <span data-ttu-id="d44ac-147">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="d44ac-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d44ac-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="d44ac-148">certificateIssuanceState</span></span>|[<span data-ttu-id="d44ac-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="d44ac-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="d44ac-150">Veröffentlichungslizenzen Zustand.</span><span class="sxs-lookup"><span data-stu-id="d44ac-150">Issuance State.</span></span> <span data-ttu-id="d44ac-151">Mögliche Werte sind: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="d44ac-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="d44ac-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="d44ac-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="d44ac-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="d44ac-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="d44ac-154">Wichtige Speicheranbieter.</span><span class="sxs-lookup"><span data-stu-id="d44ac-154">Key Storage Provider.</span></span> <span data-ttu-id="d44ac-155">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="d44ac-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="d44ac-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d44ac-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="d44ac-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d44ac-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d44ac-158">Format des Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="d44ac-158">Subject name format.</span></span> <span data-ttu-id="d44ac-159">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="d44ac-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d44ac-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="d44ac-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="d44ac-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d44ac-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d44ac-162">Subject alternative Name-Format.</span><span class="sxs-lookup"><span data-stu-id="d44ac-162">Subject alternative name format.</span></span> <span data-ttu-id="d44ac-163">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="d44ac-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d44ac-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="d44ac-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="d44ac-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="d44ac-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="d44ac-166">REVOKE-Status.</span><span class="sxs-lookup"><span data-stu-id="d44ac-166">Revoke status.</span></span> <span data-ttu-id="d44ac-167">Mögliche Werte sind: `none`, `pending`, `issued`, `failed` und `revoked`.</span><span class="sxs-lookup"><span data-stu-id="d44ac-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="d44ac-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="d44ac-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="d44ac-169">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-169">String</span></span>|<span data-ttu-id="d44ac-170">Profil der Anzeigename des Zertifikats</span><span class="sxs-lookup"><span data-stu-id="d44ac-170">Certificate profile display name</span></span>|
|<span data-ttu-id="d44ac-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d44ac-171">deviceDisplayName</span></span>|<span data-ttu-id="d44ac-172">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-172">String</span></span>|<span data-ttu-id="d44ac-173">Anzeigename des Geräts</span><span class="sxs-lookup"><span data-stu-id="d44ac-173">Device display name</span></span>|
|<span data-ttu-id="d44ac-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d44ac-174">userDisplayName</span></span>|<span data-ttu-id="d44ac-175">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-175">String</span></span>|<span data-ttu-id="d44ac-176">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="d44ac-176">User display name</span></span>|
|<span data-ttu-id="d44ac-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d44ac-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="d44ac-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44ac-178">DateTimeOffset</span></span>|<span data-ttu-id="d44ac-179">Ablaufdatum des Zertifikats</span><span class="sxs-lookup"><span data-stu-id="d44ac-179">Certificate expiry date</span></span>|
|<span data-ttu-id="d44ac-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="d44ac-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="d44ac-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44ac-181">DateTimeOffset</span></span>|<span data-ttu-id="d44ac-182">Änderung des letzten Zertifikat Veröffentlichungslizenzen</span><span class="sxs-lookup"><span data-stu-id="d44ac-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="d44ac-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="d44ac-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="d44ac-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44ac-184">DateTimeOffset</span></span>|<span data-ttu-id="d44ac-185">Änderung des letzten Zertifikat Veröffentlichungslizenzen</span><span class="sxs-lookup"><span data-stu-id="d44ac-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="d44ac-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="d44ac-186">certificateIssuer</span></span>|<span data-ttu-id="d44ac-187">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-187">String</span></span>|<span data-ttu-id="d44ac-188">Aussteller</span><span class="sxs-lookup"><span data-stu-id="d44ac-188">Issuer</span></span>|
|<span data-ttu-id="d44ac-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="d44ac-189">certificateThumbprint</span></span>|<span data-ttu-id="d44ac-190">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-190">String</span></span>|<span data-ttu-id="d44ac-191">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="d44ac-191">Thumbprint</span></span>|
|<span data-ttu-id="d44ac-192">Zertifikatsseriennummer</span><span class="sxs-lookup"><span data-stu-id="d44ac-192">certificateSerialNumber</span></span>|<span data-ttu-id="d44ac-193">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-193">String</span></span>|<span data-ttu-id="d44ac-194">Seriennummer</span><span class="sxs-lookup"><span data-stu-id="d44ac-194">Serial number</span></span>|
|<span data-ttu-id="d44ac-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="d44ac-195">certificateKeyLength</span></span>|<span data-ttu-id="d44ac-196">Int32</span><span class="sxs-lookup"><span data-stu-id="d44ac-196">Int32</span></span>|<span data-ttu-id="d44ac-197">Schlüssellänge</span><span class="sxs-lookup"><span data-stu-id="d44ac-197">Key length</span></span>|
|<span data-ttu-id="d44ac-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="d44ac-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="d44ac-199">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-199">String</span></span>|<span data-ttu-id="d44ac-200">Erweiterte Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="d44ac-200">Extended key usage</span></span>|
|<span data-ttu-id="d44ac-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="d44ac-201">certificateValidityPeriod</span></span>|<span data-ttu-id="d44ac-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d44ac-202">Int32</span></span>|<span data-ttu-id="d44ac-203">Gültigkeitsdauer</span><span class="sxs-lookup"><span data-stu-id="d44ac-203">Validity period</span></span>|
|<span data-ttu-id="d44ac-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d44ac-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="d44ac-205">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-205">String</span></span>|<span data-ttu-id="d44ac-206">Subject Name Formatzeichenfolge für benutzerdefinierte Subject Namensformate</span><span class="sxs-lookup"><span data-stu-id="d44ac-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="d44ac-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d44ac-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d44ac-208">String</span><span class="sxs-lookup"><span data-stu-id="d44ac-208">String</span></span>|<span data-ttu-id="d44ac-209">Subject alternative Name Formatzeichenfolge für benutzerdefinierte Formate</span><span class="sxs-lookup"><span data-stu-id="d44ac-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="d44ac-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="d44ac-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="d44ac-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44ac-211">DateTimeOffset</span></span>|<span data-ttu-id="d44ac-212">Veröffentlichungslizenzen Datum</span><span class="sxs-lookup"><span data-stu-id="d44ac-212">Issuance date</span></span>|
|<span data-ttu-id="d44ac-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="d44ac-213">certificateErrorCode</span></span>|<span data-ttu-id="d44ac-214">Int32</span><span class="sxs-lookup"><span data-stu-id="d44ac-214">Int32</span></span>|<span data-ttu-id="d44ac-215">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="d44ac-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="d44ac-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="d44ac-216">Response</span></span>
<span data-ttu-id="d44ac-217">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d44ac-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d44ac-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d44ac-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="d44ac-219">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d44ac-219">Request</span></span>
<span data-ttu-id="d44ac-220">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d44ac-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
Content-type: application/json
Content-length: 1517

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
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

### <a name="response"></a><span data-ttu-id="d44ac-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="d44ac-221">Response</span></span>
<span data-ttu-id="d44ac-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d44ac-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





