---
title: MacOSImportedPFXCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MacOSImportedPFXCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 61cc4160f5a91b61c117d69a81da609a7ca433ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954085"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="da483-103">MacOSImportedPFXCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="da483-103">Update macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="da483-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="da483-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da483-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da483-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da483-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="da483-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da483-107">Aktualisieren Sie die Eigenschaften eines [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="da483-107">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da483-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da483-108">Prerequisites</span></span>
<span data-ttu-id="da483-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da483-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da483-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da483-111">Permission type</span></span>|<span data-ttu-id="da483-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da483-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da483-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da483-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da483-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da483-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da483-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da483-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da483-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da483-116">Not supported.</span></span>|
|<span data-ttu-id="da483-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da483-117">Application</span></span>|<span data-ttu-id="da483-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da483-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da483-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da483-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="da483-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da483-120">Request headers</span></span>
|<span data-ttu-id="da483-121">Header</span><span class="sxs-lookup"><span data-stu-id="da483-121">Header</span></span>|<span data-ttu-id="da483-122">Wert</span><span class="sxs-lookup"><span data-stu-id="da483-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da483-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da483-123">Authorization</span></span>|<span data-ttu-id="da483-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da483-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da483-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="da483-125">Accept</span></span>|<span data-ttu-id="da483-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da483-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da483-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da483-127">Request body</span></span>
<span data-ttu-id="da483-128">Geben Sie im Textkörper Anforderung für das Objekt [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="da483-128">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="da483-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="da483-129">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="da483-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da483-130">Property</span></span>|<span data-ttu-id="da483-131">Typ</span><span class="sxs-lookup"><span data-stu-id="da483-131">Type</span></span>|<span data-ttu-id="da483-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da483-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da483-133">id</span><span class="sxs-lookup"><span data-stu-id="da483-133">id</span></span>|<span data-ttu-id="da483-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da483-134">String</span></span>|<span data-ttu-id="da483-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="da483-135">Key of the entity.</span></span> <span data-ttu-id="da483-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da483-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da483-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da483-137">lastModifiedDateTime</span></span>|<span data-ttu-id="da483-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da483-138">DateTimeOffset</span></span>|<span data-ttu-id="da483-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="da483-139">DateTime the object was last modified.</span></span> <span data-ttu-id="da483-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da483-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da483-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da483-141">roleScopeTagIds</span></span>|<span data-ttu-id="da483-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="da483-142">String collection</span></span>|<span data-ttu-id="da483-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="da483-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da483-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da483-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da483-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da483-145">supportsScopeTags</span></span>|<span data-ttu-id="da483-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="da483-146">Boolean</span></span>|<span data-ttu-id="da483-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da483-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da483-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="da483-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da483-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="da483-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da483-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da483-150">This property is read-only.</span></span> <span data-ttu-id="da483-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da483-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da483-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da483-152">createdDateTime</span></span>|<span data-ttu-id="da483-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da483-153">DateTimeOffset</span></span>|<span data-ttu-id="da483-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="da483-154">DateTime the object was created.</span></span> <span data-ttu-id="da483-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da483-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da483-156">description</span><span class="sxs-lookup"><span data-stu-id="da483-156">description</span></span>|<span data-ttu-id="da483-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da483-157">String</span></span>|<span data-ttu-id="da483-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="da483-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da483-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da483-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da483-160">displayName</span><span class="sxs-lookup"><span data-stu-id="da483-160">displayName</span></span>|<span data-ttu-id="da483-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da483-161">String</span></span>|<span data-ttu-id="da483-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="da483-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da483-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da483-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da483-164">Version</span><span class="sxs-lookup"><span data-stu-id="da483-164">version</span></span>|<span data-ttu-id="da483-165">Int32</span><span class="sxs-lookup"><span data-stu-id="da483-165">Int32</span></span>|<span data-ttu-id="da483-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="da483-166">Version of the device configuration.</span></span> <span data-ttu-id="da483-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da483-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da483-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="da483-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="da483-169">Int32</span><span class="sxs-lookup"><span data-stu-id="da483-169">Int32</span></span>|<span data-ttu-id="da483-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="da483-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="da483-171">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="da483-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="da483-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="da483-172">subjectNameFormat</span></span>|[<span data-ttu-id="da483-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="da483-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="da483-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="da483-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="da483-175">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="da483-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="da483-176">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="da483-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="da483-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="da483-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="da483-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="da483-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="da483-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="da483-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="da483-180">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="da483-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="da483-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="da483-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="da483-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="da483-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="da483-183">Int32</span><span class="sxs-lookup"><span data-stu-id="da483-183">Int32</span></span>|<span data-ttu-id="da483-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="da483-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="da483-185">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="da483-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="da483-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="da483-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="da483-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="da483-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="da483-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="da483-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="da483-189">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="da483-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="da483-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="da483-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="da483-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="da483-191">intendedPurpose</span></span>|[<span data-ttu-id="da483-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="da483-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="da483-193">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="da483-193">Not yet documented.</span></span> <span data-ttu-id="da483-194">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="da483-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="da483-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="da483-195">Response</span></span>
<span data-ttu-id="da483-196">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="da483-196">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da483-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da483-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="da483-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da483-198">Request</span></span>
<span data-ttu-id="da483-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da483-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 515

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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="da483-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="da483-200">Response</span></span>
<span data-ttu-id="da483-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da483-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





