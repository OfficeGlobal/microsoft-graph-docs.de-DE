---
title: Erstellen von windows10ImportedPFXCertificateProfile
description: Erstellen eines neuen windows10ImportedPFXCertificateProfile-Objekts.
ms.openlocfilehash: 18543d8bb7802638cb2b0840b3b1cb71271f0080
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065144"
---
# <a name="create-windows10importedpfxcertificateprofile"></a><span data-ttu-id="a0701-103">Erstellen von windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a0701-103">Create windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="a0701-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a0701-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0701-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a0701-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0701-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a0701-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0701-107">Erstellen eines neuen [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a0701-107">Create a new [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0701-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a0701-108">Prerequisites</span></span>
<span data-ttu-id="a0701-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0701-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0701-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0701-111">Permission type</span></span>|<span data-ttu-id="a0701-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0701-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0701-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0701-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0701-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0701-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0701-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0701-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0701-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0701-116">Not supported.</span></span>|
|<span data-ttu-id="a0701-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0701-117">Application</span></span>|<span data-ttu-id="a0701-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0701-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0701-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0701-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0701-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0701-120">Request headers</span></span>
|<span data-ttu-id="a0701-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a0701-121">Header</span></span>|<span data-ttu-id="a0701-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a0701-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0701-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0701-123">Authorization</span></span>|<span data-ttu-id="a0701-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a0701-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0701-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a0701-125">Accept</span></span>|<span data-ttu-id="a0701-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0701-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0701-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0701-127">Request body</span></span>
<span data-ttu-id="a0701-128">Geben Sie im Textkörper Anforderung für das Objekt windows10ImportedPFXCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a0701-128">In the request body, supply a JSON representation for the windows10ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="a0701-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows10ImportedPFXCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="a0701-129">The following table shows the properties that are required when you create the windows10ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="a0701-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a0701-130">Property</span></span>|<span data-ttu-id="a0701-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a0701-131">Type</span></span>|<span data-ttu-id="a0701-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0701-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0701-133">id</span><span class="sxs-lookup"><span data-stu-id="a0701-133">id</span></span>|<span data-ttu-id="a0701-134">String</span><span class="sxs-lookup"><span data-stu-id="a0701-134">String</span></span>|<span data-ttu-id="a0701-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a0701-135">Key of the entity.</span></span> <span data-ttu-id="a0701-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0701-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0701-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a0701-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0701-138">DateTimeOffset</span></span>|<span data-ttu-id="a0701-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a0701-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a0701-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0701-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0701-141">roleScopeTagIds</span></span>|<span data-ttu-id="a0701-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a0701-142">String collection</span></span>|<span data-ttu-id="a0701-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a0701-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0701-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0701-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a0701-145">supportsScopeTags</span></span>|<span data-ttu-id="a0701-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a0701-146">Boolean</span></span>|<span data-ttu-id="a0701-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a0701-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0701-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a0701-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0701-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a0701-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0701-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a0701-150">This property is read-only.</span></span> <span data-ttu-id="a0701-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0701-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0701-152">createdDateTime</span></span>|<span data-ttu-id="a0701-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0701-153">DateTimeOffset</span></span>|<span data-ttu-id="a0701-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a0701-154">DateTime the object was created.</span></span> <span data-ttu-id="a0701-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0701-156">description</span><span class="sxs-lookup"><span data-stu-id="a0701-156">description</span></span>|<span data-ttu-id="a0701-157">String</span><span class="sxs-lookup"><span data-stu-id="a0701-157">String</span></span>|<span data-ttu-id="a0701-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a0701-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0701-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0701-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a0701-160">displayName</span></span>|<span data-ttu-id="a0701-161">String</span><span class="sxs-lookup"><span data-stu-id="a0701-161">String</span></span>|<span data-ttu-id="a0701-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a0701-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0701-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0701-164">Version</span><span class="sxs-lookup"><span data-stu-id="a0701-164">version</span></span>|<span data-ttu-id="a0701-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a0701-165">Int32</span></span>|<span data-ttu-id="a0701-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0701-166">Version of the device configuration.</span></span> <span data-ttu-id="a0701-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0701-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a0701-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="a0701-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a0701-169">Int32</span></span>|<span data-ttu-id="a0701-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="a0701-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a0701-171">Gültige Werte 1 bis 99 Inherited aus [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0701-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a0701-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a0701-172">keyStorageProvider</span></span>|[<span data-ttu-id="a0701-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a0701-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a0701-174">Schlüssel-Speicher-Anbieter (KSP) Inherited aus [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a0701-175">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="a0701-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a0701-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a0701-176">subjectNameFormat</span></span>|[<span data-ttu-id="a0701-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a0701-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a0701-178">Zertifikat Subject Name Format geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a0701-179">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a0701-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a0701-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a0701-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a0701-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a0701-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a0701-182">Zertifikat Subject Alternative Name Typ geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a0701-183">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a0701-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a0701-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a0701-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a0701-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a0701-185">Int32</span></span>|<span data-ttu-id="a0701-186">Wert für das Zertifikat Gültigkeit Zeitraum geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0701-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a0701-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a0701-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a0701-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a0701-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a0701-189">Skalierung für das Zertifikat Gültigkeit Zeitraum geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0701-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a0701-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="a0701-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a0701-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a0701-191">intendedPurpose</span></span>|[<span data-ttu-id="a0701-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a0701-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="a0701-193">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a0701-193">Not yet documented.</span></span> <span data-ttu-id="a0701-194">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="a0701-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="a0701-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0701-195">Response</span></span>
<span data-ttu-id="a0701-196">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a0701-196">If successful, this method returns a `201 Created` response code and a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0701-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0701-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0701-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0701-198">Request</span></span>
<span data-ttu-id="a0701-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a0701-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 650

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="a0701-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0701-200">Response</span></span>
<span data-ttu-id="a0701-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0701-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 758

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```




