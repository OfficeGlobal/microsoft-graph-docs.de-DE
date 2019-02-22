---
title: Windows10pkcscertificateprofile hinzugefügt aktualisieren
description: Aktualisieren der Eigenschaften eines Windows10pkcscertificateprofile hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2991e849781155535e3af3e5e1553eda31d340ee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154838"
---
# <a name="update-windows10pkcscertificateprofile"></a><span data-ttu-id="bed1c-103">Windows10pkcscertificateprofile hinzugefügt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bed1c-103">Update windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="bed1c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bed1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bed1c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bed1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bed1c-106">Aktualisieren der Eigenschaften eines [windows10pkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bed1c-106">Update the properties of a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bed1c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bed1c-107">Prerequisites</span></span>
<span data-ttu-id="bed1c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bed1c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bed1c-110">Permission type</span></span>|<span data-ttu-id="bed1c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bed1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bed1c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bed1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bed1c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed1c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bed1c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bed1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bed1c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bed1c-115">Not supported.</span></span>|
|<span data-ttu-id="bed1c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bed1c-116">Application</span></span>|<span data-ttu-id="bed1c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bed1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bed1c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bed1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bed1c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bed1c-119">Request headers</span></span>
|<span data-ttu-id="bed1c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bed1c-120">Header</span></span>|<span data-ttu-id="bed1c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bed1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bed1c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bed1c-122">Authorization</span></span>|<span data-ttu-id="bed1c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bed1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bed1c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bed1c-124">Accept</span></span>|<span data-ttu-id="bed1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bed1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bed1c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bed1c-126">Request body</span></span>
<span data-ttu-id="bed1c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windows10pkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="bed1c-127">In the request body, supply a JSON representation for the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="bed1c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10pkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="bed1c-128">The following table shows the properties that are required when you create the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span></span>

|<span data-ttu-id="bed1c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bed1c-129">Property</span></span>|<span data-ttu-id="bed1c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="bed1c-130">Type</span></span>|<span data-ttu-id="bed1c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bed1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bed1c-132">id</span><span class="sxs-lookup"><span data-stu-id="bed1c-132">id</span></span>|<span data-ttu-id="bed1c-133">string</span><span class="sxs-lookup"><span data-stu-id="bed1c-133">String</span></span>|<span data-ttu-id="bed1c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bed1c-134">Key of the entity.</span></span> <span data-ttu-id="bed1c-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed1c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bed1c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bed1c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bed1c-137">DateTimeOffset</span></span>|<span data-ttu-id="bed1c-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bed1c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bed1c-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed1c-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="bed1c-140">roleScopeTagIds</span></span>|<span data-ttu-id="bed1c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="bed1c-141">String collection</span></span>|<span data-ttu-id="bed1c-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="bed1c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bed1c-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed1c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bed1c-144">supportsScopeTags</span></span>|<span data-ttu-id="bed1c-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bed1c-145">Boolean</span></span>|<span data-ttu-id="bed1c-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bed1c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bed1c-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="bed1c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bed1c-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="bed1c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bed1c-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bed1c-149">This property is read-only.</span></span> <span data-ttu-id="bed1c-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed1c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bed1c-151">createdDateTime</span></span>|<span data-ttu-id="bed1c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bed1c-152">DateTimeOffset</span></span>|<span data-ttu-id="bed1c-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bed1c-153">DateTime the object was created.</span></span> <span data-ttu-id="bed1c-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed1c-155">description</span><span class="sxs-lookup"><span data-stu-id="bed1c-155">description</span></span>|<span data-ttu-id="bed1c-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bed1c-156">String</span></span>|<span data-ttu-id="bed1c-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bed1c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bed1c-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed1c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bed1c-159">displayName</span></span>|<span data-ttu-id="bed1c-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bed1c-160">String</span></span>|<span data-ttu-id="bed1c-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bed1c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bed1c-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed1c-163">Version</span><span class="sxs-lookup"><span data-stu-id="bed1c-163">version</span></span>|<span data-ttu-id="bed1c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bed1c-164">Int32</span></span>|<span data-ttu-id="bed1c-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bed1c-165">Version of the device configuration.</span></span> <span data-ttu-id="bed1c-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bed1c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed1c-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="bed1c-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="bed1c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="bed1c-168">Int32</span></span>|<span data-ttu-id="bed1c-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="bed1c-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="bed1c-170">Gültige Werte 1 bis 99 geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bed1c-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bed1c-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="bed1c-171">keyStorageProvider</span></span>|[<span data-ttu-id="bed1c-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="bed1c-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="bed1c-173">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbter Schlüsselspeicheranbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="bed1c-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bed1c-174">Mögliche Werte: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="bed1c-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="bed1c-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bed1c-175">subjectNameFormat</span></span>|[<span data-ttu-id="bed1c-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bed1c-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="bed1c-177">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbtes Zertifikat für den Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="bed1c-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bed1c-178">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="bed1c-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="bed1c-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bed1c-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="bed1c-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bed1c-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bed1c-181">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbter alternativer Namenstyp des zertifikatsAntrags Tellers.</span><span class="sxs-lookup"><span data-stu-id="bed1c-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bed1c-182">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="bed1c-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="bed1c-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="bed1c-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="bed1c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="bed1c-184">Int32</span></span>|<span data-ttu-id="bed1c-185">Wert für den von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) geerbten Zertifikats Gültigkeitszeitraum</span><span class="sxs-lookup"><span data-stu-id="bed1c-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bed1c-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="bed1c-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="bed1c-187">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="bed1c-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="bed1c-188">Skalierung für den von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbten Zertifikats Gültigkeitszeitraum.</span><span class="sxs-lookup"><span data-stu-id="bed1c-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bed1c-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="bed1c-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="bed1c-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="bed1c-190">certificationAuthority</span></span>|<span data-ttu-id="bed1c-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bed1c-191">String</span></span>|<span data-ttu-id="bed1c-192">PKCS-ZertifizierungsStelle</span><span class="sxs-lookup"><span data-stu-id="bed1c-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="bed1c-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="bed1c-193">certificationAuthorityName</span></span>|<span data-ttu-id="bed1c-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bed1c-194">String</span></span>|<span data-ttu-id="bed1c-195">Name der PKCS-ZertifizierungsStelle</span><span class="sxs-lookup"><span data-stu-id="bed1c-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="bed1c-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="bed1c-196">certificateTemplateName</span></span>|<span data-ttu-id="bed1c-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bed1c-197">String</span></span>|<span data-ttu-id="bed1c-198">Name der PKCS-Zertifikatvorlage</span><span class="sxs-lookup"><span data-stu-id="bed1c-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="bed1c-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bed1c-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="bed1c-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bed1c-200">String</span></span>|<span data-ttu-id="bed1c-201">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="bed1c-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="bed1c-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="bed1c-202">extendedKeyUsages</span></span>|<span data-ttu-id="bed1c-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="bed1c-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="bed1c-204">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="bed1c-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="bed1c-205">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bed1c-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="bed1c-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="bed1c-206">Response</span></span>
<span data-ttu-id="bed1c-207">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windows10pkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bed1c-207">If successful, this method returns a `200 OK` response code and an updated [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed1c-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bed1c-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="bed1c-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bed1c-209">Request</span></span>
<span data-ttu-id="bed1c-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bed1c-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1011

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="bed1c-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="bed1c-211">Response</span></span>
<span data-ttu-id="bed1c-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bed1c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




