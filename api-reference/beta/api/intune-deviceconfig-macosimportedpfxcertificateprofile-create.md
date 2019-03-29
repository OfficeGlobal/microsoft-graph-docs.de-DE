---
title: MacOSImportedPFXCertificateProfile erstellen
description: Erstellen eines neuen macOSImportedPFXCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 646ab2bf10a296563b87692499f6f3b069da56a9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957766"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="b65cc-103">MacOSImportedPFXCertificateProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="b65cc-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="b65cc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b65cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b65cc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b65cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b65cc-106">Erstellen eines neuen [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b65cc-106">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b65cc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b65cc-107">Prerequisites</span></span>
<span data-ttu-id="b65cc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b65cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b65cc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b65cc-110">Permission type</span></span>|<span data-ttu-id="b65cc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b65cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b65cc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b65cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b65cc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b65cc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b65cc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b65cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b65cc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b65cc-115">Not supported.</span></span>|
|<span data-ttu-id="b65cc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b65cc-116">Application</span></span>|<span data-ttu-id="b65cc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b65cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b65cc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b65cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b65cc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b65cc-119">Request headers</span></span>
|<span data-ttu-id="b65cc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b65cc-120">Header</span></span>|<span data-ttu-id="b65cc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b65cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b65cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b65cc-122">Authorization</span></span>|<span data-ttu-id="b65cc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b65cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b65cc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b65cc-124">Accept</span></span>|<span data-ttu-id="b65cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b65cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b65cc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b65cc-126">Request body</span></span>
<span data-ttu-id="b65cc-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das macOSImportedPFXCertificateProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b65cc-127">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="b65cc-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSImportedPFXCertificateProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b65cc-128">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="b65cc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b65cc-129">Property</span></span>|<span data-ttu-id="b65cc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b65cc-130">Type</span></span>|<span data-ttu-id="b65cc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b65cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b65cc-132">id</span><span class="sxs-lookup"><span data-stu-id="b65cc-132">id</span></span>|<span data-ttu-id="b65cc-133">String</span><span class="sxs-lookup"><span data-stu-id="b65cc-133">String</span></span>|<span data-ttu-id="b65cc-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b65cc-134">Key of the entity.</span></span> <span data-ttu-id="b65cc-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b65cc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b65cc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b65cc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b65cc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b65cc-137">DateTimeOffset</span></span>|<span data-ttu-id="b65cc-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b65cc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b65cc-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b65cc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b65cc-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="b65cc-140">roleScopeTagIds</span></span>|<span data-ttu-id="b65cc-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b65cc-141">String collection</span></span>|<span data-ttu-id="b65cc-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="b65cc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b65cc-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b65cc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b65cc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b65cc-144">supportsScopeTags</span></span>|<span data-ttu-id="b65cc-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b65cc-145">Boolean</span></span>|<span data-ttu-id="b65cc-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b65cc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b65cc-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="b65cc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b65cc-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b65cc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b65cc-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b65cc-149">This property is read-only.</span></span> <span data-ttu-id="b65cc-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b65cc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b65cc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b65cc-151">createdDateTime</span></span>|<span data-ttu-id="b65cc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b65cc-152">DateTimeOffset</span></span>|<span data-ttu-id="b65cc-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b65cc-153">DateTime the object was created.</span></span> <span data-ttu-id="b65cc-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b65cc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b65cc-155">description</span><span class="sxs-lookup"><span data-stu-id="b65cc-155">description</span></span>|<span data-ttu-id="b65cc-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b65cc-156">String</span></span>|<span data-ttu-id="b65cc-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b65cc-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b65cc-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b65cc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b65cc-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b65cc-159">displayName</span></span>|<span data-ttu-id="b65cc-160">String</span><span class="sxs-lookup"><span data-stu-id="b65cc-160">String</span></span>|<span data-ttu-id="b65cc-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b65cc-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b65cc-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b65cc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b65cc-163">Version</span><span class="sxs-lookup"><span data-stu-id="b65cc-163">version</span></span>|<span data-ttu-id="b65cc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b65cc-164">Int32</span></span>|<span data-ttu-id="b65cc-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b65cc-165">Version of the device configuration.</span></span> <span data-ttu-id="b65cc-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b65cc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b65cc-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="b65cc-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="b65cc-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b65cc-168">Int32</span></span>|<span data-ttu-id="b65cc-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="b65cc-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b65cc-170">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b65cc-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b65cc-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b65cc-171">subjectNameFormat</span></span>|[<span data-ttu-id="b65cc-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b65cc-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="b65cc-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="b65cc-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="b65cc-174">Von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b65cc-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="b65cc-175">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="b65cc-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="b65cc-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b65cc-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b65cc-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b65cc-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b65cc-178">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="b65cc-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b65cc-179">Von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b65cc-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="b65cc-180">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b65cc-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b65cc-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b65cc-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b65cc-182">Int32</span><span class="sxs-lookup"><span data-stu-id="b65cc-182">Int32</span></span>|<span data-ttu-id="b65cc-183">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="b65cc-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b65cc-184">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b65cc-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b65cc-185">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="b65cc-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b65cc-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="b65cc-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b65cc-187">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="b65cc-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b65cc-188">Von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b65cc-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="b65cc-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="b65cc-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b65cc-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="b65cc-190">intendedPurpose</span></span>|[<span data-ttu-id="b65cc-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="b65cc-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="b65cc-192">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b65cc-192">Not yet documented.</span></span> <span data-ttu-id="b65cc-193">Mögliche Werte: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="b65cc-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="b65cc-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="b65cc-194">Response</span></span>
<span data-ttu-id="b65cc-195">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b65cc-195">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b65cc-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b65cc-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="b65cc-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b65cc-197">Request</span></span>
<span data-ttu-id="b65cc-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b65cc-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="b65cc-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="b65cc-199">Response</span></span>
<span data-ttu-id="b65cc-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b65cc-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 696

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```




