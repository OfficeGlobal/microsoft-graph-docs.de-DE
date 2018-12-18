---
title: MacOSScepCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MacOSScepCertificateProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: 1ab735b6c9d2703512a97080bc5500111c455764
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352444"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="38944-103">MacOSScepCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="38944-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="38944-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="38944-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38944-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38944-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38944-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="38944-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38944-107">Aktualisieren Sie die Eigenschaften eines [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="38944-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38944-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="38944-108">Prerequisites</span></span>
<span data-ttu-id="38944-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38944-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38944-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38944-111">Permission type</span></span>|<span data-ttu-id="38944-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38944-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38944-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38944-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38944-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38944-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38944-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38944-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38944-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38944-116">Not supported.</span></span>|
|<span data-ttu-id="38944-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38944-117">Application</span></span>|<span data-ttu-id="38944-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38944-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38944-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38944-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="38944-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38944-120">Request headers</span></span>
|<span data-ttu-id="38944-121">Header</span><span class="sxs-lookup"><span data-stu-id="38944-121">Header</span></span>|<span data-ttu-id="38944-122">Wert</span><span class="sxs-lookup"><span data-stu-id="38944-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38944-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="38944-123">Authorization</span></span>|<span data-ttu-id="38944-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="38944-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38944-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38944-125">Accept</span></span>|<span data-ttu-id="38944-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38944-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38944-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38944-127">Request body</span></span>
<span data-ttu-id="38944-128">Geben Sie im Textkörper Anforderung für das Objekt [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="38944-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="38944-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="38944-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="38944-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38944-130">Property</span></span>|<span data-ttu-id="38944-131">Typ</span><span class="sxs-lookup"><span data-stu-id="38944-131">Type</span></span>|<span data-ttu-id="38944-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38944-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38944-133">id</span><span class="sxs-lookup"><span data-stu-id="38944-133">id</span></span>|<span data-ttu-id="38944-134">String</span><span class="sxs-lookup"><span data-stu-id="38944-134">String</span></span>|<span data-ttu-id="38944-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="38944-135">Key of the entity.</span></span> <span data-ttu-id="38944-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38944-137">lastModifiedDateTime</span></span>|<span data-ttu-id="38944-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38944-138">DateTimeOffset</span></span>|<span data-ttu-id="38944-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="38944-139">DateTime the object was last modified.</span></span> <span data-ttu-id="38944-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38944-141">roleScopeTagIds</span></span>|<span data-ttu-id="38944-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="38944-142">String collection</span></span>|<span data-ttu-id="38944-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="38944-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="38944-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="38944-145">supportsScopeTags</span></span>|<span data-ttu-id="38944-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="38944-146">Boolean</span></span>|<span data-ttu-id="38944-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38944-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="38944-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="38944-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="38944-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="38944-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="38944-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="38944-150">This property is read-only.</span></span> <span data-ttu-id="38944-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38944-152">createdDateTime</span></span>|<span data-ttu-id="38944-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38944-153">DateTimeOffset</span></span>|<span data-ttu-id="38944-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="38944-154">DateTime the object was created.</span></span> <span data-ttu-id="38944-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-156">description</span><span class="sxs-lookup"><span data-stu-id="38944-156">description</span></span>|<span data-ttu-id="38944-157">String</span><span class="sxs-lookup"><span data-stu-id="38944-157">String</span></span>|<span data-ttu-id="38944-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="38944-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38944-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-160">displayName</span><span class="sxs-lookup"><span data-stu-id="38944-160">displayName</span></span>|<span data-ttu-id="38944-161">String</span><span class="sxs-lookup"><span data-stu-id="38944-161">String</span></span>|<span data-ttu-id="38944-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="38944-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38944-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-164">Version</span><span class="sxs-lookup"><span data-stu-id="38944-164">version</span></span>|<span data-ttu-id="38944-165">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-165">Int32</span></span>|<span data-ttu-id="38944-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="38944-166">Version of the device configuration.</span></span> <span data-ttu-id="38944-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="38944-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="38944-169">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-169">Int32</span></span>|<span data-ttu-id="38944-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="38944-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="38944-171">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="38944-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="38944-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="38944-172">subjectNameFormat</span></span>|[<span data-ttu-id="38944-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="38944-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="38944-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="38944-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="38944-175">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="38944-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="38944-176">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="38944-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="38944-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="38944-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="38944-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="38944-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="38944-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="38944-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="38944-180">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="38944-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="38944-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="38944-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="38944-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="38944-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="38944-183">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-183">Int32</span></span>|<span data-ttu-id="38944-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="38944-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="38944-185">Geerbt von [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="38944-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="38944-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="38944-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="38944-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="38944-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="38944-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="38944-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="38944-189">Geerbt von [MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="38944-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="38944-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="38944-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="38944-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="38944-191">scepServerUrls</span></span>|<span data-ttu-id="38944-192">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="38944-192">String collection</span></span>|<span data-ttu-id="38944-193">SCEP Server URL(s) hinzu.</span><span class="sxs-lookup"><span data-stu-id="38944-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="38944-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="38944-194">subjectNameFormatString</span></span>|<span data-ttu-id="38944-195">String</span><span class="sxs-lookup"><span data-stu-id="38944-195">String</span></span>|<span data-ttu-id="38944-196">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="38944-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="38944-197">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="38944-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="38944-198">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="38944-198">keyUsage</span></span>|[<span data-ttu-id="38944-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="38944-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="38944-200">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="38944-200">SCEP Key Usage.</span></span> <span data-ttu-id="38944-201">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="38944-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="38944-202">keySize</span><span class="sxs-lookup"><span data-stu-id="38944-202">keySize</span></span>|[<span data-ttu-id="38944-203">keySize</span><span class="sxs-lookup"><span data-stu-id="38944-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="38944-204">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="38944-204">SCEP Key Size.</span></span> <span data-ttu-id="38944-205">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="38944-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="38944-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="38944-206">hashAlgorithm</span></span>|[<span data-ttu-id="38944-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="38944-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="38944-208">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="38944-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="38944-209">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="38944-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="38944-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="38944-210">extendedKeyUsages</span></span>|<span data-ttu-id="38944-211">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="38944-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="38944-212">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="38944-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="38944-213">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="38944-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="38944-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="38944-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="38944-215">String</span><span class="sxs-lookup"><span data-stu-id="38944-215">String</span></span>|<span data-ttu-id="38944-216">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="38944-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="38944-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="38944-217">Response</span></span>
<span data-ttu-id="38944-218">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="38944-218">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38944-219">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38944-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="38944-220">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38944-220">Request</span></span>
<span data-ttu-id="38944-221">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38944-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 963

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

### <a name="response"></a><span data-ttu-id="38944-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="38944-222">Response</span></span>
<span data-ttu-id="38944-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38944-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





