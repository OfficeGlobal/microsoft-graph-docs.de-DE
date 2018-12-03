---
title: Windows10PkcsCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows10PkcsCertificateProfile-Objekts.
ms.openlocfilehash: 710b4b2abac6a4e4818e3a9f7024e3ced669e541
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061109"
---
# <a name="update-windows10pkcscertificateprofile"></a><span data-ttu-id="b2c7a-103">Windows10PkcsCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b2c7a-103">Update windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="b2c7a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2c7a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2c7a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2c7a-107">Aktualisieren Sie die Eigenschaften eines [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-107">Update the properties of a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2c7a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b2c7a-108">Prerequisites</span></span>
<span data-ttu-id="b2c7a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2c7a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b2c7a-111">Permission type</span></span>|<span data-ttu-id="b2c7a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b2c7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2c7a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b2c7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2c7a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2c7a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2c7a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b2c7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2c7a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2c7a-116">Not supported.</span></span>|
|<span data-ttu-id="b2c7a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b2c7a-117">Application</span></span>|<span data-ttu-id="b2c7a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2c7a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2c7a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2c7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b2c7a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b2c7a-120">Request headers</span></span>
|<span data-ttu-id="b2c7a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b2c7a-121">Header</span></span>|<span data-ttu-id="b2c7a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b2c7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2c7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2c7a-123">Authorization</span></span>|<span data-ttu-id="b2c7a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b2c7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2c7a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2c7a-125">Accept</span></span>|<span data-ttu-id="b2c7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2c7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2c7a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b2c7a-127">Request body</span></span>
<span data-ttu-id="b2c7a-128">Geben Sie im Textkörper Anforderung für das Objekt [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-128">In the request body, supply a JSON representation for the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="b2c7a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-129">The following table shows the properties that are required when you create the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span></span>

|<span data-ttu-id="b2c7a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2c7a-130">Property</span></span>|<span data-ttu-id="b2c7a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b2c7a-131">Type</span></span>|<span data-ttu-id="b2c7a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2c7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2c7a-133">id</span><span class="sxs-lookup"><span data-stu-id="b2c7a-133">id</span></span>|<span data-ttu-id="b2c7a-134">String</span><span class="sxs-lookup"><span data-stu-id="b2c7a-134">String</span></span>|<span data-ttu-id="b2c7a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b2c7a-135">Key of the entity.</span></span> <span data-ttu-id="b2c7a-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2c7a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2c7a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b2c7a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2c7a-138">DateTimeOffset</span></span>|<span data-ttu-id="b2c7a-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b2c7a-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2c7a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b2c7a-141">roleScopeTagIds</span></span>|<span data-ttu-id="b2c7a-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b2c7a-142">String collection</span></span>|<span data-ttu-id="b2c7a-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b2c7a-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2c7a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b2c7a-145">supportsScopeTags</span></span>|<span data-ttu-id="b2c7a-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b2c7a-146">Boolean</span></span>|<span data-ttu-id="b2c7a-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b2c7a-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b2c7a-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b2c7a-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-150">This property is read-only.</span></span> <span data-ttu-id="b2c7a-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2c7a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2c7a-152">createdDateTime</span></span>|<span data-ttu-id="b2c7a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2c7a-153">DateTimeOffset</span></span>|<span data-ttu-id="b2c7a-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-154">DateTime the object was created.</span></span> <span data-ttu-id="b2c7a-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2c7a-156">description</span><span class="sxs-lookup"><span data-stu-id="b2c7a-156">description</span></span>|<span data-ttu-id="b2c7a-157">String</span><span class="sxs-lookup"><span data-stu-id="b2c7a-157">String</span></span>|<span data-ttu-id="b2c7a-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b2c7a-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2c7a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b2c7a-160">displayName</span></span>|<span data-ttu-id="b2c7a-161">String</span><span class="sxs-lookup"><span data-stu-id="b2c7a-161">String</span></span>|<span data-ttu-id="b2c7a-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b2c7a-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2c7a-164">Version</span><span class="sxs-lookup"><span data-stu-id="b2c7a-164">version</span></span>|<span data-ttu-id="b2c7a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b2c7a-165">Int32</span></span>|<span data-ttu-id="b2c7a-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-166">Version of the device configuration.</span></span> <span data-ttu-id="b2c7a-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2c7a-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b2c7a-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b2c7a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b2c7a-169">Int32</span></span>|<span data-ttu-id="b2c7a-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b2c7a-171">Gültige Werte 1 bis 99 Inherited aus [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b2c7a-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b2c7a-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="b2c7a-172">keyStorageProvider</span></span>|[<span data-ttu-id="b2c7a-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="b2c7a-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="b2c7a-174">Schlüssel-Speicher-Anbieter (KSP) Inherited aus [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b2c7a-175">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="b2c7a-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b2c7a-176">subjectNameFormat</span></span>|[<span data-ttu-id="b2c7a-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b2c7a-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b2c7a-178">Zertifikat Subject Name Format geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b2c7a-179">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b2c7a-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b2c7a-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b2c7a-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b2c7a-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b2c7a-182">Zertifikat Subject Alternative Name Typ geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b2c7a-183">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b2c7a-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b2c7a-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b2c7a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b2c7a-185">Int32</span></span>|<span data-ttu-id="b2c7a-186">Wert für das Zertifikat Gültigkeit Zeitraum geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b2c7a-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b2c7a-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b2c7a-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b2c7a-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b2c7a-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b2c7a-189">Skalierung für das Zertifikat Gültigkeit Zeitraum geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b2c7a-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b2c7a-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b2c7a-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="b2c7a-191">certificationAuthority</span></span>|<span data-ttu-id="b2c7a-192">String</span><span class="sxs-lookup"><span data-stu-id="b2c7a-192">String</span></span>|<span data-ttu-id="b2c7a-193">PKCS-Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="b2c7a-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="b2c7a-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="b2c7a-194">certificationAuthorityName</span></span>|<span data-ttu-id="b2c7a-195">String</span><span class="sxs-lookup"><span data-stu-id="b2c7a-195">String</span></span>|<span data-ttu-id="b2c7a-196">Name der Zertifizierungsstelle PKCS</span><span class="sxs-lookup"><span data-stu-id="b2c7a-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="b2c7a-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="b2c7a-197">certificateTemplateName</span></span>|<span data-ttu-id="b2c7a-198">String</span><span class="sxs-lookup"><span data-stu-id="b2c7a-198">String</span></span>|<span data-ttu-id="b2c7a-199">Name der PKCS Zertifikatsvorlage</span><span class="sxs-lookup"><span data-stu-id="b2c7a-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="b2c7a-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b2c7a-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b2c7a-201">String</span><span class="sxs-lookup"><span data-stu-id="b2c7a-201">String</span></span>|<span data-ttu-id="b2c7a-202">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b2c7a-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b2c7a-203">extendedKeyUsages</span></span>|<span data-ttu-id="b2c7a-204">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b2c7a-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b2c7a-205">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b2c7a-206">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-206">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b2c7a-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2c7a-207">Response</span></span>
<span data-ttu-id="b2c7a-208">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-208">If successful, this method returns a `200 OK` response code and an updated [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2c7a-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b2c7a-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2c7a-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2c7a-210">Request</span></span>
<span data-ttu-id="b2c7a-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1005

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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b2c7a-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2c7a-212">Response</span></span>
<span data-ttu-id="b2c7a-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2c7a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1183

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```





