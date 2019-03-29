---
title: MacOSScepCertificateProfile erstellen
description: Erstellen eines neuen macOSScepCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c40bd6835f562c52fa03720472802a569e8a5c23
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972893"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="7ad34-103">MacOSScepCertificateProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="7ad34-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="7ad34-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ad34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ad34-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7ad34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ad34-106">Erstellen eines neuen [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7ad34-106">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ad34-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7ad34-107">Prerequisites</span></span>
<span data-ttu-id="7ad34-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ad34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ad34-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ad34-110">Permission type</span></span>|<span data-ttu-id="7ad34-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ad34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ad34-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ad34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ad34-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ad34-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ad34-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ad34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ad34-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ad34-115">Not supported.</span></span>|
|<span data-ttu-id="7ad34-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ad34-116">Application</span></span>|<span data-ttu-id="7ad34-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ad34-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ad34-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7ad34-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ad34-119">Request headers</span></span>
|<span data-ttu-id="7ad34-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7ad34-120">Header</span></span>|<span data-ttu-id="7ad34-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7ad34-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ad34-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ad34-122">Authorization</span></span>|<span data-ttu-id="7ad34-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7ad34-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ad34-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7ad34-124">Accept</span></span>|<span data-ttu-id="7ad34-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ad34-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ad34-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ad34-126">Request body</span></span>
<span data-ttu-id="7ad34-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das macOSScepCertificateProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="7ad34-127">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="7ad34-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSScepCertificateProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7ad34-128">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="7ad34-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7ad34-129">Property</span></span>|<span data-ttu-id="7ad34-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7ad34-130">Type</span></span>|<span data-ttu-id="7ad34-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ad34-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ad34-132">id</span><span class="sxs-lookup"><span data-stu-id="7ad34-132">id</span></span>|<span data-ttu-id="7ad34-133">String</span><span class="sxs-lookup"><span data-stu-id="7ad34-133">String</span></span>|<span data-ttu-id="7ad34-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7ad34-134">Key of the entity.</span></span> <span data-ttu-id="7ad34-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ad34-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad34-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ad34-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7ad34-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ad34-137">DateTimeOffset</span></span>|<span data-ttu-id="7ad34-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7ad34-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7ad34-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ad34-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad34-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="7ad34-140">roleScopeTagIds</span></span>|<span data-ttu-id="7ad34-141">String collection</span><span class="sxs-lookup"><span data-stu-id="7ad34-141">String collection</span></span>|<span data-ttu-id="7ad34-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="7ad34-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7ad34-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ad34-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad34-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7ad34-144">supportsScopeTags</span></span>|<span data-ttu-id="7ad34-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7ad34-145">Boolean</span></span>|<span data-ttu-id="7ad34-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ad34-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7ad34-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="7ad34-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7ad34-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="7ad34-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7ad34-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7ad34-149">This property is read-only.</span></span> <span data-ttu-id="7ad34-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ad34-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad34-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ad34-151">createdDateTime</span></span>|<span data-ttu-id="7ad34-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ad34-152">DateTimeOffset</span></span>|<span data-ttu-id="7ad34-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7ad34-153">DateTime the object was created.</span></span> <span data-ttu-id="7ad34-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ad34-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad34-155">description</span><span class="sxs-lookup"><span data-stu-id="7ad34-155">description</span></span>|<span data-ttu-id="7ad34-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ad34-156">String</span></span>|<span data-ttu-id="7ad34-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7ad34-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7ad34-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ad34-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad34-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7ad34-159">displayName</span></span>|<span data-ttu-id="7ad34-160">String</span><span class="sxs-lookup"><span data-stu-id="7ad34-160">String</span></span>|<span data-ttu-id="7ad34-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7ad34-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7ad34-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ad34-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad34-163">Version</span><span class="sxs-lookup"><span data-stu-id="7ad34-163">version</span></span>|<span data-ttu-id="7ad34-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7ad34-164">Int32</span></span>|<span data-ttu-id="7ad34-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7ad34-165">Version of the device configuration.</span></span> <span data-ttu-id="7ad34-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ad34-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad34-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="7ad34-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="7ad34-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7ad34-168">Int32</span></span>|<span data-ttu-id="7ad34-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="7ad34-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7ad34-170">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ad34-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7ad34-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7ad34-171">subjectNameFormat</span></span>|[<span data-ttu-id="7ad34-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7ad34-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="7ad34-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="7ad34-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="7ad34-174">Von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="7ad34-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7ad34-175">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="7ad34-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="7ad34-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7ad34-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7ad34-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7ad34-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7ad34-178">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="7ad34-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="7ad34-179">Von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="7ad34-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7ad34-180">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="7ad34-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7ad34-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7ad34-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7ad34-182">Int32</span><span class="sxs-lookup"><span data-stu-id="7ad34-182">Int32</span></span>|<span data-ttu-id="7ad34-183">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="7ad34-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7ad34-184">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ad34-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7ad34-185">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="7ad34-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7ad34-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="7ad34-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7ad34-187">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="7ad34-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7ad34-188">Von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="7ad34-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7ad34-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="7ad34-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7ad34-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="7ad34-190">scepServerUrls</span></span>|<span data-ttu-id="7ad34-191">String collection</span><span class="sxs-lookup"><span data-stu-id="7ad34-191">String collection</span></span>|<span data-ttu-id="7ad34-192">SCEP-Server-URL (s).</span><span class="sxs-lookup"><span data-stu-id="7ad34-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="7ad34-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7ad34-193">subjectNameFormatString</span></span>|<span data-ttu-id="7ad34-194">String</span><span class="sxs-lookup"><span data-stu-id="7ad34-194">String</span></span>|<span data-ttu-id="7ad34-195">Benutzerdefiniertes Format, das mit SubjectNameFormat = Custom verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="7ad34-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="7ad34-196">Beispiel: CN = {{Email Adresse}}, E = {Email Adresse}}, OU = Enterprise users, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="7ad34-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="7ad34-197">keyUsage</span><span class="sxs-lookup"><span data-stu-id="7ad34-197">keyUsage</span></span>|[<span data-ttu-id="7ad34-198">keyUsages</span><span class="sxs-lookup"><span data-stu-id="7ad34-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="7ad34-199">SCEP-Schlüsselverwendung.</span><span class="sxs-lookup"><span data-stu-id="7ad34-199">SCEP Key Usage.</span></span> <span data-ttu-id="7ad34-200">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="7ad34-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="7ad34-201">keySize</span><span class="sxs-lookup"><span data-stu-id="7ad34-201">keySize</span></span>|[<span data-ttu-id="7ad34-202">keySize</span><span class="sxs-lookup"><span data-stu-id="7ad34-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="7ad34-203">SCEP-Schlüsselgröße.</span><span class="sxs-lookup"><span data-stu-id="7ad34-203">SCEP Key Size.</span></span> <span data-ttu-id="7ad34-204">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="7ad34-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="7ad34-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="7ad34-205">hashAlgorithm</span></span>|[<span data-ttu-id="7ad34-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="7ad34-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="7ad34-207">SCEP-Hash Algorithmus.</span><span class="sxs-lookup"><span data-stu-id="7ad34-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="7ad34-208">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="7ad34-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="7ad34-209">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="7ad34-209">extendedKeyUsages</span></span>|<span data-ttu-id="7ad34-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="7ad34-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="7ad34-211">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="7ad34-211">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="7ad34-212">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7ad34-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7ad34-213">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7ad34-213">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7ad34-214">String</span><span class="sxs-lookup"><span data-stu-id="7ad34-214">String</span></span>|<span data-ttu-id="7ad34-215">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="7ad34-215">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="7ad34-216">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7ad34-216">certificateStore</span></span>|[<span data-ttu-id="7ad34-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7ad34-217">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="7ad34-218">Zielspeicher Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="7ad34-218">Target store certificate.</span></span> <span data-ttu-id="7ad34-219">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="7ad34-219">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="7ad34-220">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="7ad34-220">customSubjectAlternativeNames</span></span>|<span data-ttu-id="7ad34-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="7ad34-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="7ad34-222">Einstellungen für benutzerdefinierte Alternative AntragsTellernamen.</span><span class="sxs-lookup"><span data-stu-id="7ad34-222">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="7ad34-223">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7ad34-223">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7ad34-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad34-224">Response</span></span>
<span data-ttu-id="7ad34-225">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7ad34-225">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ad34-226">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ad34-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ad34-227">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad34-227">Request</span></span>
<span data-ttu-id="7ad34-228">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ad34-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7ad34-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad34-229">Response</span></span>
<span data-ttu-id="7ad34-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ad34-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```




