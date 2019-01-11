---
title: IosPkcsCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosPkcsCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1cd5426ad8d07984ff25209326d613add09cc000
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817801"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="c9846-103">IosPkcsCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c9846-103">Update iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="c9846-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c9846-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9846-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9846-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9846-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9846-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9846-107">Aktualisieren Sie die Eigenschaften eines [IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9846-107">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9846-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9846-108">Prerequisites</span></span>
<span data-ttu-id="c9846-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9846-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9846-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9846-111">Permission type</span></span>|<span data-ttu-id="c9846-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9846-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9846-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9846-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9846-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9846-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9846-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9846-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9846-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9846-116">Not supported.</span></span>|
|<span data-ttu-id="c9846-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9846-117">Application</span></span>|<span data-ttu-id="c9846-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9846-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9846-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9846-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c9846-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9846-120">Request headers</span></span>
|<span data-ttu-id="c9846-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c9846-121">Header</span></span>|<span data-ttu-id="c9846-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c9846-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9846-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9846-123">Authorization</span></span>|<span data-ttu-id="c9846-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9846-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9846-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c9846-125">Accept</span></span>|<span data-ttu-id="c9846-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9846-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9846-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9846-127">Request body</span></span>
<span data-ttu-id="c9846-128">Geben Sie im Textkörper Anforderung für das Objekt [IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c9846-128">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="c9846-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="c9846-129">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="c9846-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9846-130">Property</span></span>|<span data-ttu-id="c9846-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c9846-131">Type</span></span>|<span data-ttu-id="c9846-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9846-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9846-133">id</span><span class="sxs-lookup"><span data-stu-id="c9846-133">id</span></span>|<span data-ttu-id="c9846-134">String</span><span class="sxs-lookup"><span data-stu-id="c9846-134">String</span></span>|<span data-ttu-id="c9846-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c9846-135">Key of the entity.</span></span> <span data-ttu-id="c9846-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9846-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9846-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c9846-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9846-138">DateTimeOffset</span></span>|<span data-ttu-id="c9846-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9846-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c9846-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9846-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9846-141">roleScopeTagIds</span></span>|<span data-ttu-id="c9846-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c9846-142">String collection</span></span>|<span data-ttu-id="c9846-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c9846-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9846-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9846-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9846-145">supportsScopeTags</span></span>|<span data-ttu-id="c9846-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9846-146">Boolean</span></span>|<span data-ttu-id="c9846-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9846-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9846-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c9846-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9846-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c9846-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9846-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c9846-150">This property is read-only.</span></span> <span data-ttu-id="c9846-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9846-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9846-152">createdDateTime</span></span>|<span data-ttu-id="c9846-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9846-153">DateTimeOffset</span></span>|<span data-ttu-id="c9846-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9846-154">DateTime the object was created.</span></span> <span data-ttu-id="c9846-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9846-156">description</span><span class="sxs-lookup"><span data-stu-id="c9846-156">description</span></span>|<span data-ttu-id="c9846-157">String</span><span class="sxs-lookup"><span data-stu-id="c9846-157">String</span></span>|<span data-ttu-id="c9846-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c9846-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9846-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9846-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c9846-160">displayName</span></span>|<span data-ttu-id="c9846-161">String</span><span class="sxs-lookup"><span data-stu-id="c9846-161">String</span></span>|<span data-ttu-id="c9846-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c9846-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9846-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9846-164">Version</span><span class="sxs-lookup"><span data-stu-id="c9846-164">version</span></span>|<span data-ttu-id="c9846-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c9846-165">Int32</span></span>|<span data-ttu-id="c9846-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c9846-166">Version of the device configuration.</span></span> <span data-ttu-id="c9846-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9846-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c9846-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="c9846-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c9846-169">Int32</span></span>|<span data-ttu-id="c9846-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="c9846-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c9846-171">Gültige Werte 1 bis 99 Inherited aus [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c9846-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c9846-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c9846-172">subjectNameFormat</span></span>|[<span data-ttu-id="c9846-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c9846-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="c9846-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="c9846-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="c9846-175">Geerbt von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c9846-176">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="c9846-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="c9846-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c9846-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c9846-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c9846-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c9846-179">Alternativer Antragstellername Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="c9846-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="c9846-180">Geerbt von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c9846-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c9846-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c9846-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c9846-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c9846-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c9846-183">Int32</span></span>|<span data-ttu-id="c9846-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="c9846-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c9846-185">Geerbt von [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c9846-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c9846-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c9846-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c9846-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c9846-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c9846-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="c9846-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c9846-189">Geerbt von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c9846-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c9846-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="c9846-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c9846-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="c9846-191">certificationAuthority</span></span>|<span data-ttu-id="c9846-192">String</span><span class="sxs-lookup"><span data-stu-id="c9846-192">String</span></span>|<span data-ttu-id="c9846-193">PKCS Zertifizierungsstelle.</span><span class="sxs-lookup"><span data-stu-id="c9846-193">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="c9846-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="c9846-194">certificationAuthorityName</span></span>|<span data-ttu-id="c9846-195">String</span><span class="sxs-lookup"><span data-stu-id="c9846-195">String</span></span>|<span data-ttu-id="c9846-196">Name der Zertifizierungsstelle PKCS.</span><span class="sxs-lookup"><span data-stu-id="c9846-196">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="c9846-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="c9846-197">certificateTemplateName</span></span>|<span data-ttu-id="c9846-198">String</span><span class="sxs-lookup"><span data-stu-id="c9846-198">String</span></span>|<span data-ttu-id="c9846-199">Name der PKCS Zertifikatsvorlage.</span><span class="sxs-lookup"><span data-stu-id="c9846-199">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="c9846-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c9846-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c9846-201">String</span><span class="sxs-lookup"><span data-stu-id="c9846-201">String</span></span>|<span data-ttu-id="c9846-202">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="c9846-202">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="c9846-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9846-203">Response</span></span>
<span data-ttu-id="c9846-204">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c9846-204">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9846-205">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9846-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9846-206">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9846-206">Request</span></span>
<span data-ttu-id="c9846-207">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9846-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 761

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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="c9846-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9846-208">Response</span></span>
<span data-ttu-id="c9846-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9846-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





