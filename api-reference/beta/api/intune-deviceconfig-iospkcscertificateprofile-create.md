---
title: Iospkcscertificateprofile hinzugefügt erstellen
description: Erstellen eines neuen Iospkcscertificateprofile hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 78b0622befa7e9cac32bb6f6f95803d731a0060d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171540"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="abd52-103">Iospkcscertificateprofile hinzugefügt erstellen</span><span class="sxs-lookup"><span data-stu-id="abd52-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="abd52-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="abd52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abd52-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="abd52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abd52-106">Erstellen eines neuen [iospkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-iospkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="abd52-106">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abd52-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="abd52-107">Prerequisites</span></span>
<span data-ttu-id="abd52-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="abd52-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abd52-110">Permission type</span></span>|<span data-ttu-id="abd52-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abd52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abd52-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abd52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abd52-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abd52-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abd52-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abd52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abd52-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abd52-115">Not supported.</span></span>|
|<span data-ttu-id="abd52-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abd52-116">Application</span></span>|<span data-ttu-id="abd52-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abd52-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abd52-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abd52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="abd52-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abd52-119">Request headers</span></span>
|<span data-ttu-id="abd52-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="abd52-120">Header</span></span>|<span data-ttu-id="abd52-121">Wert</span><span class="sxs-lookup"><span data-stu-id="abd52-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abd52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="abd52-122">Authorization</span></span>|<span data-ttu-id="abd52-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="abd52-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abd52-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="abd52-124">Accept</span></span>|<span data-ttu-id="abd52-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abd52-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abd52-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abd52-126">Request body</span></span>
<span data-ttu-id="abd52-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das Iospkcscertificateprofile hinzugefügt-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="abd52-127">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="abd52-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der Iospkcscertificateprofile hinzugefügt erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="abd52-128">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="abd52-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abd52-129">Property</span></span>|<span data-ttu-id="abd52-130">Typ</span><span class="sxs-lookup"><span data-stu-id="abd52-130">Type</span></span>|<span data-ttu-id="abd52-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abd52-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abd52-132">id</span><span class="sxs-lookup"><span data-stu-id="abd52-132">id</span></span>|<span data-ttu-id="abd52-133">string</span><span class="sxs-lookup"><span data-stu-id="abd52-133">String</span></span>|<span data-ttu-id="abd52-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="abd52-134">Key of the entity.</span></span> <span data-ttu-id="abd52-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abd52-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abd52-136">lastModifiedDateTime</span></span>|<span data-ttu-id="abd52-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abd52-137">DateTimeOffset</span></span>|<span data-ttu-id="abd52-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="abd52-138">DateTime the object was last modified.</span></span> <span data-ttu-id="abd52-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abd52-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="abd52-140">roleScopeTagIds</span></span>|<span data-ttu-id="abd52-141">String collection</span><span class="sxs-lookup"><span data-stu-id="abd52-141">String collection</span></span>|<span data-ttu-id="abd52-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="abd52-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="abd52-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abd52-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="abd52-144">supportsScopeTags</span></span>|<span data-ttu-id="abd52-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="abd52-145">Boolean</span></span>|<span data-ttu-id="abd52-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="abd52-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="abd52-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="abd52-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="abd52-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="abd52-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="abd52-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="abd52-149">This property is read-only.</span></span> <span data-ttu-id="abd52-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abd52-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abd52-151">createdDateTime</span></span>|<span data-ttu-id="abd52-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abd52-152">DateTimeOffset</span></span>|<span data-ttu-id="abd52-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="abd52-153">DateTime the object was created.</span></span> <span data-ttu-id="abd52-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abd52-155">description</span><span class="sxs-lookup"><span data-stu-id="abd52-155">description</span></span>|<span data-ttu-id="abd52-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abd52-156">String</span></span>|<span data-ttu-id="abd52-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="abd52-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="abd52-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abd52-159">displayName</span><span class="sxs-lookup"><span data-stu-id="abd52-159">displayName</span></span>|<span data-ttu-id="abd52-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abd52-160">String</span></span>|<span data-ttu-id="abd52-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="abd52-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="abd52-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abd52-163">Version</span><span class="sxs-lookup"><span data-stu-id="abd52-163">version</span></span>|<span data-ttu-id="abd52-164">Int32</span><span class="sxs-lookup"><span data-stu-id="abd52-164">Int32</span></span>|<span data-ttu-id="abd52-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="abd52-165">Version of the device configuration.</span></span> <span data-ttu-id="abd52-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abd52-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abd52-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="abd52-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="abd52-168">Int32</span><span class="sxs-lookup"><span data-stu-id="abd52-168">Int32</span></span>|<span data-ttu-id="abd52-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="abd52-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="abd52-170">Gültige Werte 1 bis 99 geerbt von [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="abd52-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="abd52-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="abd52-171">subjectNameFormat</span></span>|[<span data-ttu-id="abd52-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="abd52-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="abd52-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="abd52-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="abd52-174">Von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="abd52-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="abd52-175">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="abd52-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="abd52-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="abd52-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="abd52-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="abd52-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="abd52-178">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="abd52-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="abd52-179">Von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="abd52-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="abd52-180">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="abd52-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="abd52-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="abd52-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="abd52-182">Int32</span><span class="sxs-lookup"><span data-stu-id="abd52-182">Int32</span></span>|<span data-ttu-id="abd52-183">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="abd52-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="abd52-184">Geerbt von [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="abd52-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="abd52-185">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="abd52-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="abd52-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="abd52-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="abd52-187">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="abd52-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="abd52-188">Von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="abd52-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="abd52-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="abd52-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="abd52-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="abd52-190">certificationAuthority</span></span>|<span data-ttu-id="abd52-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abd52-191">String</span></span>|<span data-ttu-id="abd52-192">PKCS-ZertifizierungsStelle.</span><span class="sxs-lookup"><span data-stu-id="abd52-192">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="abd52-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="abd52-193">certificationAuthorityName</span></span>|<span data-ttu-id="abd52-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abd52-194">String</span></span>|<span data-ttu-id="abd52-195">Name der PKCS-ZertifizierungsStelle.</span><span class="sxs-lookup"><span data-stu-id="abd52-195">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="abd52-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="abd52-196">certificateTemplateName</span></span>|<span data-ttu-id="abd52-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abd52-197">String</span></span>|<span data-ttu-id="abd52-198">Name der PKCS-Zertifikatvorlage.</span><span class="sxs-lookup"><span data-stu-id="abd52-198">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="abd52-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="abd52-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="abd52-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abd52-200">String</span></span>|<span data-ttu-id="abd52-201">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="abd52-201">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="abd52-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="abd52-202">Response</span></span>
<span data-ttu-id="abd52-203">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iospkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-iospkcscertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="abd52-203">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abd52-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abd52-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="abd52-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abd52-205">Request</span></span>
<span data-ttu-id="abd52-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abd52-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 761

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="abd52-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="abd52-207">Response</span></span>
<span data-ttu-id="abd52-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abd52-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 933

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




