---
title: ManagedDeviceCertificateState aktualisieren
description: Aktualisieren der Eigenschaften eines managedDeviceCertificateState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a360e35e83712178d71256bdd6f389081e4047c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171701"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="871ed-103">ManagedDeviceCertificateState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="871ed-103">Update managedDeviceCertificateState</span></span>

> <span data-ttu-id="871ed-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="871ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="871ed-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="871ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="871ed-106">Aktualisieren der Eigenschaften eines [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="871ed-106">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="871ed-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="871ed-107">Prerequisites</span></span>
<span data-ttu-id="871ed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="871ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="871ed-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="871ed-110">Permission type</span></span>|<span data-ttu-id="871ed-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="871ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="871ed-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="871ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="871ed-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="871ed-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="871ed-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="871ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="871ed-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="871ed-115">Not supported.</span></span>|
|<span data-ttu-id="871ed-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="871ed-116">Application</span></span>|<span data-ttu-id="871ed-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="871ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="871ed-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="871ed-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="871ed-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="871ed-119">Request headers</span></span>
|<span data-ttu-id="871ed-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="871ed-120">Header</span></span>|<span data-ttu-id="871ed-121">Wert</span><span class="sxs-lookup"><span data-stu-id="871ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="871ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="871ed-122">Authorization</span></span>|<span data-ttu-id="871ed-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="871ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="871ed-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="871ed-124">Accept</span></span>|<span data-ttu-id="871ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="871ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="871ed-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="871ed-126">Request body</span></span>
<span data-ttu-id="871ed-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="871ed-127">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="871ed-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="871ed-128">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="871ed-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="871ed-129">Property</span></span>|<span data-ttu-id="871ed-130">Typ</span><span class="sxs-lookup"><span data-stu-id="871ed-130">Type</span></span>|<span data-ttu-id="871ed-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="871ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="871ed-132">id</span><span class="sxs-lookup"><span data-stu-id="871ed-132">id</span></span>|<span data-ttu-id="871ed-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-133">String</span></span>|<span data-ttu-id="871ed-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="871ed-134">Key of the entity.</span></span>|
|<span data-ttu-id="871ed-135">Deviceplatform wurde</span><span class="sxs-lookup"><span data-stu-id="871ed-135">devicePlatform</span></span>|[<span data-ttu-id="871ed-136">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="871ed-136">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="871ed-137">Geräteplattform.</span><span class="sxs-lookup"><span data-stu-id="871ed-137">Device platform.</span></span> <span data-ttu-id="871ed-138">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="871ed-138">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="871ed-139">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="871ed-139">certificateKeyUsage</span></span>|[<span data-ttu-id="871ed-140">keyUsages</span><span class="sxs-lookup"><span data-stu-id="871ed-140">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="871ed-141">Schlüsselverwendung.</span><span class="sxs-lookup"><span data-stu-id="871ed-141">Key usage.</span></span> <span data-ttu-id="871ed-142">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="871ed-142">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="871ed-143">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="871ed-143">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="871ed-144">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="871ed-144">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="871ed-145">Gültigkeitszeitraum Einheiten.</span><span class="sxs-lookup"><span data-stu-id="871ed-145">Validity period units.</span></span> <span data-ttu-id="871ed-146">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="871ed-146">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="871ed-147">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="871ed-147">certificateIssuanceState</span></span>|[<span data-ttu-id="871ed-148">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="871ed-148">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="871ed-149">VeröffentlichungsStatus.</span><span class="sxs-lookup"><span data-stu-id="871ed-149">Issuance State.</span></span> <span data-ttu-id="871ed-150">Mögliche Werte sind: `unknown`, `challengeIssued`, `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` `enrollmentNotNeeded` `revoked`,,,,,,,, `removedFromCollection`,, `installed` ,,,,,, `renewVerified` `installFailed` `issueFailed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="871ed-150">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="871ed-151">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="871ed-151">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="871ed-152">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="871ed-152">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="871ed-153">Schlüsselspeicheranbieter.</span><span class="sxs-lookup"><span data-stu-id="871ed-153">Key Storage Provider.</span></span> <span data-ttu-id="871ed-154">Mögliche Werte: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="871ed-154">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="871ed-155">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="871ed-155">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="871ed-156">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="871ed-156">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="871ed-157">Format des Antragstellernamens.</span><span class="sxs-lookup"><span data-stu-id="871ed-157">Subject name format.</span></span> <span data-ttu-id="871ed-158">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="871ed-158">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="871ed-159">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="871ed-159">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="871ed-160">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="871ed-160">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="871ed-161">Format für alternative Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="871ed-161">Subject alternative name format.</span></span> <span data-ttu-id="871ed-162">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="871ed-162">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="871ed-163">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="871ed-163">certificateRevokeStatus</span></span>|[<span data-ttu-id="871ed-164">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="871ed-164">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="871ed-165">Widerrufen des Status.</span><span class="sxs-lookup"><span data-stu-id="871ed-165">Revoke status.</span></span> <span data-ttu-id="871ed-166">Mögliche Werte: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="871ed-166">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="871ed-167">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="871ed-167">certificateProfileDisplayName</span></span>|<span data-ttu-id="871ed-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-168">String</span></span>|<span data-ttu-id="871ed-169">Anzeigename des Zertifikat Profils</span><span class="sxs-lookup"><span data-stu-id="871ed-169">Certificate profile display name</span></span>|
|<span data-ttu-id="871ed-170">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="871ed-170">deviceDisplayName</span></span>|<span data-ttu-id="871ed-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-171">String</span></span>|<span data-ttu-id="871ed-172">Anzeigename des Geräts</span><span class="sxs-lookup"><span data-stu-id="871ed-172">Device display name</span></span>|
|<span data-ttu-id="871ed-173">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="871ed-173">userDisplayName</span></span>|<span data-ttu-id="871ed-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-174">String</span></span>|<span data-ttu-id="871ed-175">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="871ed-175">User display name</span></span>|
|<span data-ttu-id="871ed-176">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="871ed-176">certificateExpirationDateTime</span></span>|<span data-ttu-id="871ed-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="871ed-177">DateTimeOffset</span></span>|<span data-ttu-id="871ed-178">Zertifikatablaufdatum</span><span class="sxs-lookup"><span data-stu-id="871ed-178">Certificate expiry date</span></span>|
|<span data-ttu-id="871ed-179">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="871ed-179">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="871ed-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="871ed-180">DateTimeOffset</span></span>|<span data-ttu-id="871ed-181">Letzte Änderung des Zertifikat Ausstellungs Status</span><span class="sxs-lookup"><span data-stu-id="871ed-181">Last certificate issuance state change</span></span>|
|<span data-ttu-id="871ed-182">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="871ed-182">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="871ed-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="871ed-183">DateTimeOffset</span></span>|<span data-ttu-id="871ed-184">Letzte Änderung des Zertifikat Ausstellungs Status</span><span class="sxs-lookup"><span data-stu-id="871ed-184">Last certificate issuance state change</span></span>|
|<span data-ttu-id="871ed-185">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="871ed-185">certificateIssuer</span></span>|<span data-ttu-id="871ed-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-186">String</span></span>|<span data-ttu-id="871ed-187">Aussteller</span><span class="sxs-lookup"><span data-stu-id="871ed-187">Issuer</span></span>|
|<span data-ttu-id="871ed-188">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="871ed-188">certificateThumbprint</span></span>|<span data-ttu-id="871ed-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-189">String</span></span>|<span data-ttu-id="871ed-190">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="871ed-190">Thumbprint</span></span>|
|<span data-ttu-id="871ed-191">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="871ed-191">certificateSerialNumber</span></span>|<span data-ttu-id="871ed-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-192">String</span></span>|<span data-ttu-id="871ed-193">Seriennummer</span><span class="sxs-lookup"><span data-stu-id="871ed-193">Serial number</span></span>|
|<span data-ttu-id="871ed-194">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="871ed-194">certificateKeyLength</span></span>|<span data-ttu-id="871ed-195">Int32</span><span class="sxs-lookup"><span data-stu-id="871ed-195">Int32</span></span>|<span data-ttu-id="871ed-196">Schlüssellänge</span><span class="sxs-lookup"><span data-stu-id="871ed-196">Key length</span></span>|
|<span data-ttu-id="871ed-197">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="871ed-197">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="871ed-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-198">String</span></span>|<span data-ttu-id="871ed-199">Erweiterte Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="871ed-199">Extended key usage</span></span>|
|<span data-ttu-id="871ed-200">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="871ed-200">certificateValidityPeriod</span></span>|<span data-ttu-id="871ed-201">Int32</span><span class="sxs-lookup"><span data-stu-id="871ed-201">Int32</span></span>|<span data-ttu-id="871ed-202">Gültigkeitszeitraum</span><span class="sxs-lookup"><span data-stu-id="871ed-202">Validity period</span></span>|
|<span data-ttu-id="871ed-203">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="871ed-203">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="871ed-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-204">String</span></span>|<span data-ttu-id="871ed-205">Formatzeichenfolge für den Antragstellernamen für benutzerdefinierte Antragstellernamen Formate</span><span class="sxs-lookup"><span data-stu-id="871ed-205">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="871ed-206">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="871ed-206">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="871ed-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="871ed-207">String</span></span>|<span data-ttu-id="871ed-208">Formatzeichenfolge für alternative Antragstellernamen für benutzerdefinierte Formate</span><span class="sxs-lookup"><span data-stu-id="871ed-208">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="871ed-209">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="871ed-209">certificateIssuanceDateTime</span></span>|<span data-ttu-id="871ed-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="871ed-210">DateTimeOffset</span></span>|<span data-ttu-id="871ed-211">Veröffentlichungsdatum</span><span class="sxs-lookup"><span data-stu-id="871ed-211">Issuance date</span></span>|
|<span data-ttu-id="871ed-212">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="871ed-212">certificateErrorCode</span></span>|<span data-ttu-id="871ed-213">Int32</span><span class="sxs-lookup"><span data-stu-id="871ed-213">Int32</span></span>|<span data-ttu-id="871ed-214">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="871ed-214">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="871ed-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="871ed-215">Response</span></span>
<span data-ttu-id="871ed-216">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="871ed-216">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="871ed-217">Beispiel</span><span class="sxs-lookup"><span data-stu-id="871ed-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="871ed-218">Anforderung</span><span class="sxs-lookup"><span data-stu-id="871ed-218">Request</span></span>
<span data-ttu-id="871ed-219">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="871ed-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
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

### <a name="response"></a><span data-ttu-id="871ed-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="871ed-220">Response</span></span>
<span data-ttu-id="871ed-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="871ed-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




