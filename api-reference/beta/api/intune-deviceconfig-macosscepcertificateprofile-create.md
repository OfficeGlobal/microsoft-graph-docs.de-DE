---
title: Erstellen von macOSScepCertificateProfile
description: Erstellen eines neuen MacOSScepCertificateProfile-Objekts.
ms.openlocfilehash: a0dfb409217ce38fca9b966c642c09ff89887f61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065227"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="6c129-103">Erstellen von macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6c129-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="6c129-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6c129-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c129-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c129-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c129-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6c129-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c129-107">Erstellen eines neuen [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c129-107">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c129-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6c129-108">Prerequisites</span></span>
<span data-ttu-id="6c129-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c129-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c129-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c129-111">Permission type</span></span>|<span data-ttu-id="6c129-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c129-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c129-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c129-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c129-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c129-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c129-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c129-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c129-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c129-116">Not supported.</span></span>|
|<span data-ttu-id="6c129-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c129-117">Application</span></span>|<span data-ttu-id="6c129-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c129-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c129-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c129-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c129-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c129-120">Request headers</span></span>
|<span data-ttu-id="6c129-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c129-121">Header</span></span>|<span data-ttu-id="6c129-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6c129-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c129-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c129-123">Authorization</span></span>|<span data-ttu-id="6c129-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6c129-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c129-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c129-125">Accept</span></span>|<span data-ttu-id="6c129-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c129-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c129-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c129-127">Request body</span></span>
<span data-ttu-id="6c129-128">Geben Sie im Textkörper Anforderung für das Objekt MacOSScepCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6c129-128">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="6c129-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MacOSScepCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="6c129-129">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="6c129-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c129-130">Property</span></span>|<span data-ttu-id="6c129-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6c129-131">Type</span></span>|<span data-ttu-id="6c129-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c129-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c129-133">id</span><span class="sxs-lookup"><span data-stu-id="6c129-133">id</span></span>|<span data-ttu-id="6c129-134">String</span><span class="sxs-lookup"><span data-stu-id="6c129-134">String</span></span>|<span data-ttu-id="6c129-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6c129-135">Key of the entity.</span></span> <span data-ttu-id="6c129-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c129-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c129-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6c129-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c129-138">DateTimeOffset</span></span>|<span data-ttu-id="6c129-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c129-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6c129-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c129-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c129-141">roleScopeTagIds</span></span>|<span data-ttu-id="6c129-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6c129-142">String collection</span></span>|<span data-ttu-id="6c129-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="6c129-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c129-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c129-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c129-145">supportsScopeTags</span></span>|<span data-ttu-id="6c129-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6c129-146">Boolean</span></span>|<span data-ttu-id="6c129-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c129-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c129-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="6c129-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c129-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6c129-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c129-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6c129-150">This property is read-only.</span></span> <span data-ttu-id="6c129-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c129-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c129-152">createdDateTime</span></span>|<span data-ttu-id="6c129-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c129-153">DateTimeOffset</span></span>|<span data-ttu-id="6c129-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c129-154">DateTime the object was created.</span></span> <span data-ttu-id="6c129-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c129-156">description</span><span class="sxs-lookup"><span data-stu-id="6c129-156">description</span></span>|<span data-ttu-id="6c129-157">String</span><span class="sxs-lookup"><span data-stu-id="6c129-157">String</span></span>|<span data-ttu-id="6c129-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6c129-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c129-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c129-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6c129-160">displayName</span></span>|<span data-ttu-id="6c129-161">String</span><span class="sxs-lookup"><span data-stu-id="6c129-161">String</span></span>|<span data-ttu-id="6c129-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6c129-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c129-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c129-164">Version</span><span class="sxs-lookup"><span data-stu-id="6c129-164">version</span></span>|<span data-ttu-id="6c129-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6c129-165">Int32</span></span>|<span data-ttu-id="6c129-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c129-166">Version of the device configuration.</span></span> <span data-ttu-id="6c129-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c129-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6c129-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="6c129-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6c129-169">Int32</span></span>|<span data-ttu-id="6c129-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="6c129-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6c129-171">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6c129-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6c129-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6c129-172">subjectNameFormat</span></span>|[<span data-ttu-id="6c129-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6c129-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="6c129-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="6c129-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="6c129-175">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="6c129-176">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="6c129-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="6c129-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6c129-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6c129-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6c129-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6c129-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="6c129-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="6c129-180">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="6c129-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="6c129-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="6c129-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6c129-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6c129-183">Int32</span><span class="sxs-lookup"><span data-stu-id="6c129-183">Int32</span></span>|<span data-ttu-id="6c129-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="6c129-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="6c129-185">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6c129-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6c129-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6c129-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6c129-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6c129-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6c129-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="6c129-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="6c129-189">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6c129-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="6c129-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="6c129-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6c129-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="6c129-191">scepServerUrls</span></span>|<span data-ttu-id="6c129-192">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6c129-192">String collection</span></span>|<span data-ttu-id="6c129-193">SCEP Server URL(s) hinzu.</span><span class="sxs-lookup"><span data-stu-id="6c129-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="6c129-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6c129-194">subjectNameFormatString</span></span>|<span data-ttu-id="6c129-195">String</span><span class="sxs-lookup"><span data-stu-id="6c129-195">String</span></span>|<span data-ttu-id="6c129-196">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="6c129-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="6c129-197">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="6c129-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="6c129-198">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="6c129-198">keyUsage</span></span>|[<span data-ttu-id="6c129-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="6c129-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="6c129-200">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="6c129-200">SCEP Key Usage.</span></span> <span data-ttu-id="6c129-201">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="6c129-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="6c129-202">keySize</span><span class="sxs-lookup"><span data-stu-id="6c129-202">keySize</span></span>|[<span data-ttu-id="6c129-203">keySize</span><span class="sxs-lookup"><span data-stu-id="6c129-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="6c129-204">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="6c129-204">SCEP Key Size.</span></span> <span data-ttu-id="6c129-205">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="6c129-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="6c129-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6c129-206">hashAlgorithm</span></span>|[<span data-ttu-id="6c129-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="6c129-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="6c129-208">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="6c129-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="6c129-209">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="6c129-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="6c129-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6c129-210">extendedKeyUsages</span></span>|<span data-ttu-id="6c129-211">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6c129-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="6c129-212">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="6c129-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="6c129-213">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6c129-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6c129-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6c129-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="6c129-215">String</span><span class="sxs-lookup"><span data-stu-id="6c129-215">String</span></span>|<span data-ttu-id="6c129-216">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="6c129-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="6c129-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c129-217">Response</span></span>
<span data-ttu-id="6c129-218">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6c129-218">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c129-219">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c129-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c129-220">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c129-220">Request</span></span>
<span data-ttu-id="6c129-221">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c129-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1029

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="6c129-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c129-222">Response</span></span>
<span data-ttu-id="6c129-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c129-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1137

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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





