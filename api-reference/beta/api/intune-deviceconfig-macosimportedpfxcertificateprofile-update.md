---
title: MacOSImportedPFXCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MacOSImportedPFXCertificateProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: 842b680ad6f8d2337bfecfcd270252d216499807
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321966"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="338d2-103">MacOSImportedPFXCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="338d2-103">Update macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="338d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="338d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="338d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="338d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="338d2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="338d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="338d2-107">Aktualisieren Sie die Eigenschaften eines [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="338d2-107">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="338d2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="338d2-108">Prerequisites</span></span>
<span data-ttu-id="338d2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="338d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="338d2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="338d2-111">Permission type</span></span>|<span data-ttu-id="338d2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="338d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="338d2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="338d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="338d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="338d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="338d2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="338d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="338d2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="338d2-116">Not supported.</span></span>|
|<span data-ttu-id="338d2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="338d2-117">Application</span></span>|<span data-ttu-id="338d2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="338d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="338d2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="338d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="338d2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="338d2-120">Request headers</span></span>
|<span data-ttu-id="338d2-121">Header</span><span class="sxs-lookup"><span data-stu-id="338d2-121">Header</span></span>|<span data-ttu-id="338d2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="338d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="338d2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="338d2-123">Authorization</span></span>|<span data-ttu-id="338d2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="338d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="338d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="338d2-125">Accept</span></span>|<span data-ttu-id="338d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="338d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="338d2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="338d2-127">Request body</span></span>
<span data-ttu-id="338d2-128">Geben Sie im Textkörper Anforderung für das Objekt [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="338d2-128">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="338d2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="338d2-129">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="338d2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="338d2-130">Property</span></span>|<span data-ttu-id="338d2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="338d2-131">Type</span></span>|<span data-ttu-id="338d2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="338d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="338d2-133">id</span><span class="sxs-lookup"><span data-stu-id="338d2-133">id</span></span>|<span data-ttu-id="338d2-134">String</span><span class="sxs-lookup"><span data-stu-id="338d2-134">String</span></span>|<span data-ttu-id="338d2-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="338d2-135">Key of the entity.</span></span> <span data-ttu-id="338d2-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="338d2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="338d2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="338d2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="338d2-138">DateTimeOffset</span></span>|<span data-ttu-id="338d2-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="338d2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="338d2-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="338d2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="338d2-141">roleScopeTagIds</span></span>|<span data-ttu-id="338d2-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="338d2-142">String collection</span></span>|<span data-ttu-id="338d2-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="338d2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="338d2-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="338d2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="338d2-145">supportsScopeTags</span></span>|<span data-ttu-id="338d2-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="338d2-146">Boolean</span></span>|<span data-ttu-id="338d2-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="338d2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="338d2-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="338d2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="338d2-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="338d2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="338d2-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="338d2-150">This property is read-only.</span></span> <span data-ttu-id="338d2-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="338d2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="338d2-152">createdDateTime</span></span>|<span data-ttu-id="338d2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="338d2-153">DateTimeOffset</span></span>|<span data-ttu-id="338d2-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="338d2-154">DateTime the object was created.</span></span> <span data-ttu-id="338d2-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="338d2-156">description</span><span class="sxs-lookup"><span data-stu-id="338d2-156">description</span></span>|<span data-ttu-id="338d2-157">String</span><span class="sxs-lookup"><span data-stu-id="338d2-157">String</span></span>|<span data-ttu-id="338d2-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="338d2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="338d2-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="338d2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="338d2-160">displayName</span></span>|<span data-ttu-id="338d2-161">String</span><span class="sxs-lookup"><span data-stu-id="338d2-161">String</span></span>|<span data-ttu-id="338d2-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="338d2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="338d2-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="338d2-164">Version</span><span class="sxs-lookup"><span data-stu-id="338d2-164">version</span></span>|<span data-ttu-id="338d2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="338d2-165">Int32</span></span>|<span data-ttu-id="338d2-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="338d2-166">Version of the device configuration.</span></span> <span data-ttu-id="338d2-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="338d2-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="338d2-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="338d2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="338d2-169">Int32</span></span>|<span data-ttu-id="338d2-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="338d2-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="338d2-171">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="338d2-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="338d2-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="338d2-172">subjectNameFormat</span></span>|[<span data-ttu-id="338d2-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="338d2-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="338d2-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="338d2-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="338d2-175">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="338d2-176">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="338d2-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="338d2-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="338d2-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="338d2-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="338d2-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="338d2-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="338d2-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="338d2-180">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="338d2-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="338d2-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="338d2-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="338d2-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="338d2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="338d2-183">Int32</span></span>|<span data-ttu-id="338d2-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="338d2-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="338d2-185">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="338d2-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="338d2-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="338d2-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="338d2-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="338d2-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="338d2-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="338d2-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="338d2-189">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="338d2-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="338d2-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="338d2-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="338d2-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="338d2-191">intendedPurpose</span></span>|[<span data-ttu-id="338d2-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="338d2-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="338d2-193">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="338d2-193">Not yet documented.</span></span> <span data-ttu-id="338d2-194">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="338d2-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="338d2-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="338d2-195">Response</span></span>
<span data-ttu-id="338d2-196">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="338d2-196">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="338d2-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="338d2-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="338d2-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="338d2-198">Request</span></span>
<span data-ttu-id="338d2-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="338d2-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="338d2-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="338d2-200">Response</span></span>
<span data-ttu-id="338d2-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="338d2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





