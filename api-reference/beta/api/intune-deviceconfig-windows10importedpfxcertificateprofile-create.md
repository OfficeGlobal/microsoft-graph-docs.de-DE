---
title: Windows10ImportedPFXCertificateProfile erstellen
description: Erstellen eines neuen windows10ImportedPFXCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a986e258e0d0b61bf178c27a3a14e30743d8d312
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145339"
---
# <a name="create-windows10importedpfxcertificateprofile"></a><span data-ttu-id="97685-103">Windows10ImportedPFXCertificateProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="97685-103">Create windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="97685-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97685-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97685-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="97685-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97685-106">Erstellen eines neuen [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="97685-106">Create a new [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97685-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="97685-107">Prerequisites</span></span>
<span data-ttu-id="97685-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="97685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="97685-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97685-110">Permission type</span></span>|<span data-ttu-id="97685-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97685-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97685-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97685-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97685-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97685-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97685-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97685-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97685-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97685-115">Not supported.</span></span>|
|<span data-ttu-id="97685-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97685-116">Application</span></span>|<span data-ttu-id="97685-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97685-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97685-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97685-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="97685-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97685-119">Request headers</span></span>
|<span data-ttu-id="97685-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97685-120">Header</span></span>|<span data-ttu-id="97685-121">Wert</span><span class="sxs-lookup"><span data-stu-id="97685-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97685-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97685-122">Authorization</span></span>|<span data-ttu-id="97685-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="97685-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97685-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="97685-124">Accept</span></span>|<span data-ttu-id="97685-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97685-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97685-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97685-126">Request body</span></span>
<span data-ttu-id="97685-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windows10ImportedPFXCertificateProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="97685-127">In the request body, supply a JSON representation for the windows10ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="97685-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10ImportedPFXCertificateProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="97685-128">The following table shows the properties that are required when you create the windows10ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="97685-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97685-129">Property</span></span>|<span data-ttu-id="97685-130">Typ</span><span class="sxs-lookup"><span data-stu-id="97685-130">Type</span></span>|<span data-ttu-id="97685-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97685-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97685-132">id</span><span class="sxs-lookup"><span data-stu-id="97685-132">id</span></span>|<span data-ttu-id="97685-133">string</span><span class="sxs-lookup"><span data-stu-id="97685-133">String</span></span>|<span data-ttu-id="97685-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="97685-134">Key of the entity.</span></span> <span data-ttu-id="97685-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97685-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97685-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97685-136">lastModifiedDateTime</span></span>|<span data-ttu-id="97685-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97685-137">DateTimeOffset</span></span>|<span data-ttu-id="97685-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="97685-138">DateTime the object was last modified.</span></span> <span data-ttu-id="97685-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97685-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97685-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="97685-140">roleScopeTagIds</span></span>|<span data-ttu-id="97685-141">String collection</span><span class="sxs-lookup"><span data-stu-id="97685-141">String collection</span></span>|<span data-ttu-id="97685-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="97685-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="97685-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97685-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97685-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="97685-144">supportsScopeTags</span></span>|<span data-ttu-id="97685-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97685-145">Boolean</span></span>|<span data-ttu-id="97685-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97685-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="97685-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="97685-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="97685-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="97685-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="97685-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97685-149">This property is read-only.</span></span> <span data-ttu-id="97685-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97685-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97685-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97685-151">createdDateTime</span></span>|<span data-ttu-id="97685-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97685-152">DateTimeOffset</span></span>|<span data-ttu-id="97685-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="97685-153">DateTime the object was created.</span></span> <span data-ttu-id="97685-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97685-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97685-155">description</span><span class="sxs-lookup"><span data-stu-id="97685-155">description</span></span>|<span data-ttu-id="97685-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97685-156">String</span></span>|<span data-ttu-id="97685-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="97685-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="97685-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97685-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97685-159">displayName</span><span class="sxs-lookup"><span data-stu-id="97685-159">displayName</span></span>|<span data-ttu-id="97685-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97685-160">String</span></span>|<span data-ttu-id="97685-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="97685-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="97685-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97685-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97685-163">Version</span><span class="sxs-lookup"><span data-stu-id="97685-163">version</span></span>|<span data-ttu-id="97685-164">Int32</span><span class="sxs-lookup"><span data-stu-id="97685-164">Int32</span></span>|<span data-ttu-id="97685-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="97685-165">Version of the device configuration.</span></span> <span data-ttu-id="97685-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97685-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97685-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="97685-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="97685-168">Int32</span><span class="sxs-lookup"><span data-stu-id="97685-168">Int32</span></span>|<span data-ttu-id="97685-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="97685-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="97685-170">Gültige Werte 1 bis 99 geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="97685-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="97685-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="97685-171">keyStorageProvider</span></span>|[<span data-ttu-id="97685-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="97685-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="97685-173">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbter Schlüsselspeicheranbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="97685-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="97685-174">Mögliche Werte: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="97685-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="97685-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="97685-175">subjectNameFormat</span></span>|[<span data-ttu-id="97685-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="97685-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="97685-177">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbtes Zertifikat für den Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="97685-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="97685-178">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="97685-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="97685-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="97685-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="97685-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="97685-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="97685-181">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbter alternativer Namenstyp des zertifikatsAntrags Tellers.</span><span class="sxs-lookup"><span data-stu-id="97685-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="97685-182">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="97685-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="97685-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="97685-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="97685-184">Int32</span><span class="sxs-lookup"><span data-stu-id="97685-184">Int32</span></span>|<span data-ttu-id="97685-185">Wert für den von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) geerbten Zertifikats Gültigkeitszeitraum</span><span class="sxs-lookup"><span data-stu-id="97685-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="97685-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="97685-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="97685-187">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="97685-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="97685-188">Skalierung für den von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbten Zertifikats Gültigkeitszeitraum.</span><span class="sxs-lookup"><span data-stu-id="97685-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="97685-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="97685-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="97685-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="97685-190">intendedPurpose</span></span>|[<span data-ttu-id="97685-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="97685-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="97685-192">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="97685-192">Not yet documented.</span></span> <span data-ttu-id="97685-193">Mögliche Werte: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="97685-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="97685-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="97685-194">Response</span></span>
<span data-ttu-id="97685-195">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="97685-195">If successful, this method returns a `201 Created` response code and a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97685-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97685-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="97685-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97685-197">Request</span></span>
<span data-ttu-id="97685-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97685-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 586

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="97685-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="97685-199">Response</span></span>
<span data-ttu-id="97685-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97685-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




