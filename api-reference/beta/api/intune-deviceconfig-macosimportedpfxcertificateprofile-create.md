---
title: Erstellen von macOSImportedPFXCertificateProfile
description: Erstellen eines neuen MacOSImportedPFXCertificateProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fa14580bd62d42e3706d7a7f422f46832e78cf02
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408264"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="a56bd-103">Erstellen von macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a56bd-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="a56bd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a56bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a56bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a56bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a56bd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a56bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a56bd-107">Erstellen eines neuen [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a56bd-107">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a56bd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a56bd-108">Prerequisites</span></span>
<span data-ttu-id="a56bd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a56bd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a56bd-111">Permission type</span></span>|<span data-ttu-id="a56bd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a56bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a56bd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a56bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a56bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a56bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a56bd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a56bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a56bd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a56bd-116">Not supported.</span></span>|
|<span data-ttu-id="a56bd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a56bd-117">Application</span></span>|<span data-ttu-id="a56bd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a56bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a56bd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a56bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a56bd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a56bd-120">Request headers</span></span>
|<span data-ttu-id="a56bd-121">Header</span><span class="sxs-lookup"><span data-stu-id="a56bd-121">Header</span></span>|<span data-ttu-id="a56bd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a56bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a56bd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a56bd-123">Authorization</span></span>|<span data-ttu-id="a56bd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a56bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a56bd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a56bd-125">Accept</span></span>|<span data-ttu-id="a56bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a56bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a56bd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a56bd-127">Request body</span></span>
<span data-ttu-id="a56bd-128">Geben Sie im Textkörper Anforderung für das Objekt MacOSImportedPFXCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a56bd-128">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="a56bd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MacOSImportedPFXCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="a56bd-129">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="a56bd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a56bd-130">Property</span></span>|<span data-ttu-id="a56bd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a56bd-131">Type</span></span>|<span data-ttu-id="a56bd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a56bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a56bd-133">id</span><span class="sxs-lookup"><span data-stu-id="a56bd-133">id</span></span>|<span data-ttu-id="a56bd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a56bd-134">String</span></span>|<span data-ttu-id="a56bd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a56bd-135">Key of the entity.</span></span> <span data-ttu-id="a56bd-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56bd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a56bd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a56bd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a56bd-138">DateTimeOffset</span></span>|<span data-ttu-id="a56bd-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a56bd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a56bd-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56bd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a56bd-141">roleScopeTagIds</span></span>|<span data-ttu-id="a56bd-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a56bd-142">String collection</span></span>|<span data-ttu-id="a56bd-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a56bd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a56bd-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56bd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a56bd-145">supportsScopeTags</span></span>|<span data-ttu-id="a56bd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a56bd-146">Boolean</span></span>|<span data-ttu-id="a56bd-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a56bd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a56bd-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a56bd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a56bd-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a56bd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a56bd-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a56bd-150">This property is read-only.</span></span> <span data-ttu-id="a56bd-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56bd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a56bd-152">createdDateTime</span></span>|<span data-ttu-id="a56bd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a56bd-153">DateTimeOffset</span></span>|<span data-ttu-id="a56bd-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a56bd-154">DateTime the object was created.</span></span> <span data-ttu-id="a56bd-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56bd-156">description</span><span class="sxs-lookup"><span data-stu-id="a56bd-156">description</span></span>|<span data-ttu-id="a56bd-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a56bd-157">String</span></span>|<span data-ttu-id="a56bd-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a56bd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a56bd-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56bd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a56bd-160">displayName</span></span>|<span data-ttu-id="a56bd-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a56bd-161">String</span></span>|<span data-ttu-id="a56bd-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a56bd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a56bd-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56bd-164">Version</span><span class="sxs-lookup"><span data-stu-id="a56bd-164">version</span></span>|<span data-ttu-id="a56bd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a56bd-165">Int32</span></span>|<span data-ttu-id="a56bd-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a56bd-166">Version of the device configuration.</span></span> <span data-ttu-id="a56bd-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56bd-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a56bd-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="a56bd-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a56bd-169">Int32</span></span>|<span data-ttu-id="a56bd-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="a56bd-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a56bd-171">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a56bd-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a56bd-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a56bd-172">subjectNameFormat</span></span>|[<span data-ttu-id="a56bd-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a56bd-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="a56bd-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="a56bd-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="a56bd-175">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="a56bd-176">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="a56bd-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="a56bd-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a56bd-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a56bd-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a56bd-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a56bd-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="a56bd-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a56bd-180">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="a56bd-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a56bd-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a56bd-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a56bd-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a56bd-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a56bd-183">Int32</span></span>|<span data-ttu-id="a56bd-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a56bd-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a56bd-185">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a56bd-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a56bd-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a56bd-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a56bd-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a56bd-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a56bd-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a56bd-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a56bd-189">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a56bd-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="a56bd-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="a56bd-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a56bd-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a56bd-191">intendedPurpose</span></span>|[<span data-ttu-id="a56bd-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a56bd-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="a56bd-193">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a56bd-193">Not yet documented.</span></span> <span data-ttu-id="a56bd-194">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="a56bd-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="a56bd-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="a56bd-195">Response</span></span>
<span data-ttu-id="a56bd-196">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a56bd-196">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a56bd-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a56bd-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="a56bd-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a56bd-198">Request</span></span>
<span data-ttu-id="a56bd-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a56bd-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a56bd-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="a56bd-200">Response</span></span>
<span data-ttu-id="a56bd-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a56bd-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




