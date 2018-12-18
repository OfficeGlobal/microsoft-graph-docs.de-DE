---
title: Windows10ImportedPFXCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows10ImportedPFXCertificateProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: 4da4107d9a72bef94c806b83c542856881c9db1e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337786"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="53cab-103">Windows10ImportedPFXCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="53cab-103">Update windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="53cab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53cab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53cab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53cab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53cab-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="53cab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53cab-107">Aktualisieren Sie die Eigenschaften eines [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="53cab-107">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53cab-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53cab-108">Prerequisites</span></span>
<span data-ttu-id="53cab-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53cab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53cab-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53cab-111">Permission type</span></span>|<span data-ttu-id="53cab-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53cab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53cab-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53cab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53cab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53cab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53cab-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53cab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53cab-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53cab-116">Not supported.</span></span>|
|<span data-ttu-id="53cab-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53cab-117">Application</span></span>|<span data-ttu-id="53cab-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53cab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53cab-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53cab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="53cab-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53cab-120">Request headers</span></span>
|<span data-ttu-id="53cab-121">Header</span><span class="sxs-lookup"><span data-stu-id="53cab-121">Header</span></span>|<span data-ttu-id="53cab-122">Wert</span><span class="sxs-lookup"><span data-stu-id="53cab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53cab-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="53cab-123">Authorization</span></span>|<span data-ttu-id="53cab-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53cab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53cab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53cab-125">Accept</span></span>|<span data-ttu-id="53cab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53cab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53cab-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53cab-127">Request body</span></span>
<span data-ttu-id="53cab-128">Geben Sie im Textkörper Anforderung für das Objekt [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="53cab-128">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="53cab-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="53cab-129">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="53cab-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53cab-130">Property</span></span>|<span data-ttu-id="53cab-131">Typ</span><span class="sxs-lookup"><span data-stu-id="53cab-131">Type</span></span>|<span data-ttu-id="53cab-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53cab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53cab-133">id</span><span class="sxs-lookup"><span data-stu-id="53cab-133">id</span></span>|<span data-ttu-id="53cab-134">String</span><span class="sxs-lookup"><span data-stu-id="53cab-134">String</span></span>|<span data-ttu-id="53cab-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="53cab-135">Key of the entity.</span></span> <span data-ttu-id="53cab-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53cab-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53cab-137">lastModifiedDateTime</span></span>|<span data-ttu-id="53cab-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53cab-138">DateTimeOffset</span></span>|<span data-ttu-id="53cab-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="53cab-139">DateTime the object was last modified.</span></span> <span data-ttu-id="53cab-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53cab-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53cab-141">roleScopeTagIds</span></span>|<span data-ttu-id="53cab-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="53cab-142">String collection</span></span>|<span data-ttu-id="53cab-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="53cab-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="53cab-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53cab-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="53cab-145">supportsScopeTags</span></span>|<span data-ttu-id="53cab-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="53cab-146">Boolean</span></span>|<span data-ttu-id="53cab-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53cab-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="53cab-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="53cab-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="53cab-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="53cab-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="53cab-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="53cab-150">This property is read-only.</span></span> <span data-ttu-id="53cab-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53cab-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53cab-152">createdDateTime</span></span>|<span data-ttu-id="53cab-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53cab-153">DateTimeOffset</span></span>|<span data-ttu-id="53cab-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="53cab-154">DateTime the object was created.</span></span> <span data-ttu-id="53cab-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53cab-156">description</span><span class="sxs-lookup"><span data-stu-id="53cab-156">description</span></span>|<span data-ttu-id="53cab-157">String</span><span class="sxs-lookup"><span data-stu-id="53cab-157">String</span></span>|<span data-ttu-id="53cab-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="53cab-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="53cab-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53cab-160">displayName</span><span class="sxs-lookup"><span data-stu-id="53cab-160">displayName</span></span>|<span data-ttu-id="53cab-161">String</span><span class="sxs-lookup"><span data-stu-id="53cab-161">String</span></span>|<span data-ttu-id="53cab-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="53cab-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="53cab-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53cab-164">Version</span><span class="sxs-lookup"><span data-stu-id="53cab-164">version</span></span>|<span data-ttu-id="53cab-165">Int32</span><span class="sxs-lookup"><span data-stu-id="53cab-165">Int32</span></span>|<span data-ttu-id="53cab-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="53cab-166">Version of the device configuration.</span></span> <span data-ttu-id="53cab-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53cab-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="53cab-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="53cab-169">Int32</span><span class="sxs-lookup"><span data-stu-id="53cab-169">Int32</span></span>|<span data-ttu-id="53cab-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="53cab-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="53cab-171">Gültige Werte 1 bis 99 Inherited aus [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="53cab-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="53cab-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="53cab-172">keyStorageProvider</span></span>|[<span data-ttu-id="53cab-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="53cab-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="53cab-174">Schlüssel-Speicher-Anbieter (KSP) Inherited aus [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="53cab-175">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="53cab-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="53cab-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="53cab-176">subjectNameFormat</span></span>|[<span data-ttu-id="53cab-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="53cab-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="53cab-178">Zertifikat Subject Name Format geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="53cab-179">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="53cab-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="53cab-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="53cab-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="53cab-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="53cab-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="53cab-182">Zertifikat Subject Alternative Name Typ geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="53cab-183">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="53cab-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="53cab-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="53cab-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="53cab-185">Int32</span><span class="sxs-lookup"><span data-stu-id="53cab-185">Int32</span></span>|<span data-ttu-id="53cab-186">Wert für das Zertifikat Gültigkeit Zeitraum geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="53cab-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="53cab-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="53cab-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="53cab-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="53cab-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="53cab-189">Skalierung für das Zertifikat Gültigkeit Zeitraum geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="53cab-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="53cab-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="53cab-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="53cab-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="53cab-191">intendedPurpose</span></span>|[<span data-ttu-id="53cab-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="53cab-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="53cab-193">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="53cab-193">Not yet documented.</span></span> <span data-ttu-id="53cab-194">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="53cab-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="53cab-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="53cab-195">Response</span></span>
<span data-ttu-id="53cab-196">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="53cab-196">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53cab-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53cab-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="53cab-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53cab-198">Request</span></span>
<span data-ttu-id="53cab-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53cab-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 573

{
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

### <a name="response"></a><span data-ttu-id="53cab-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="53cab-200">Response</span></span>
<span data-ttu-id="53cab-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53cab-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





