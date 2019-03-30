---
title: Windows10pkcscertificateprofile hinzugefügt erstellen
description: Erstellen eines neuen Windows10pkcscertificateprofile hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5e4d10264e24df678c45770f1b660f05e99eb5b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988455"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="33b13-103">Windows10pkcscertificateprofile hinzugefügt erstellen</span><span class="sxs-lookup"><span data-stu-id="33b13-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="33b13-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33b13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33b13-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="33b13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33b13-106">Erstellen eines neuen [windows10pkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33b13-106">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33b13-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33b13-107">Prerequisites</span></span>
<span data-ttu-id="33b13-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33b13-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33b13-110">Permission type</span></span>|<span data-ttu-id="33b13-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33b13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33b13-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33b13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33b13-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b13-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33b13-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33b13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33b13-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33b13-115">Not supported.</span></span>|
|<span data-ttu-id="33b13-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33b13-116">Application</span></span>|<span data-ttu-id="33b13-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33b13-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33b13-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33b13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="33b13-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33b13-119">Request headers</span></span>
|<span data-ttu-id="33b13-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="33b13-120">Header</span></span>|<span data-ttu-id="33b13-121">Wert</span><span class="sxs-lookup"><span data-stu-id="33b13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33b13-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33b13-122">Authorization</span></span>|<span data-ttu-id="33b13-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33b13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33b13-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33b13-124">Accept</span></span>|<span data-ttu-id="33b13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33b13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33b13-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33b13-126">Request body</span></span>
<span data-ttu-id="33b13-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das Windows10pkcscertificateprofile hinzugefügt-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="33b13-127">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="33b13-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der Windows10pkcscertificateprofile hinzugefügt erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="33b13-128">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="33b13-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33b13-129">Property</span></span>|<span data-ttu-id="33b13-130">Typ</span><span class="sxs-lookup"><span data-stu-id="33b13-130">Type</span></span>|<span data-ttu-id="33b13-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33b13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33b13-132">id</span><span class="sxs-lookup"><span data-stu-id="33b13-132">id</span></span>|<span data-ttu-id="33b13-133">String</span><span class="sxs-lookup"><span data-stu-id="33b13-133">String</span></span>|<span data-ttu-id="33b13-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33b13-134">Key of the entity.</span></span> <span data-ttu-id="33b13-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b13-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b13-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33b13-136">lastModifiedDateTime</span></span>|<span data-ttu-id="33b13-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33b13-137">DateTimeOffset</span></span>|<span data-ttu-id="33b13-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33b13-138">DateTime the object was last modified.</span></span> <span data-ttu-id="33b13-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b13-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b13-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="33b13-140">roleScopeTagIds</span></span>|<span data-ttu-id="33b13-141">String collection</span><span class="sxs-lookup"><span data-stu-id="33b13-141">String collection</span></span>|<span data-ttu-id="33b13-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="33b13-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33b13-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b13-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b13-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="33b13-144">supportsScopeTags</span></span>|<span data-ttu-id="33b13-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="33b13-145">Boolean</span></span>|<span data-ttu-id="33b13-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33b13-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33b13-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="33b13-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33b13-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="33b13-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33b13-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33b13-149">This property is read-only.</span></span> <span data-ttu-id="33b13-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b13-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b13-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33b13-151">createdDateTime</span></span>|<span data-ttu-id="33b13-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33b13-152">DateTimeOffset</span></span>|<span data-ttu-id="33b13-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33b13-153">DateTime the object was created.</span></span> <span data-ttu-id="33b13-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b13-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b13-155">description</span><span class="sxs-lookup"><span data-stu-id="33b13-155">description</span></span>|<span data-ttu-id="33b13-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33b13-156">String</span></span>|<span data-ttu-id="33b13-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33b13-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33b13-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b13-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b13-159">displayName</span><span class="sxs-lookup"><span data-stu-id="33b13-159">displayName</span></span>|<span data-ttu-id="33b13-160">String</span><span class="sxs-lookup"><span data-stu-id="33b13-160">String</span></span>|<span data-ttu-id="33b13-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33b13-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33b13-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b13-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b13-163">Version</span><span class="sxs-lookup"><span data-stu-id="33b13-163">version</span></span>|<span data-ttu-id="33b13-164">Int32</span><span class="sxs-lookup"><span data-stu-id="33b13-164">Int32</span></span>|<span data-ttu-id="33b13-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="33b13-165">Version of the device configuration.</span></span> <span data-ttu-id="33b13-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b13-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b13-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="33b13-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="33b13-168">Int32</span><span class="sxs-lookup"><span data-stu-id="33b13-168">Int32</span></span>|<span data-ttu-id="33b13-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="33b13-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="33b13-170">Gültige Werte 1 bis 99 geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="33b13-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="33b13-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="33b13-171">keyStorageProvider</span></span>|[<span data-ttu-id="33b13-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="33b13-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="33b13-173">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbter Schlüsselspeicheranbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="33b13-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="33b13-174">Mögliche Werte sind: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="33b13-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="33b13-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="33b13-175">subjectNameFormat</span></span>|[<span data-ttu-id="33b13-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="33b13-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="33b13-177">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbtes Zertifikat für den Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="33b13-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="33b13-178">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="33b13-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="33b13-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="33b13-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="33b13-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="33b13-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="33b13-181">Von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbter alternativer Namenstyp des zertifikatsAntrags Tellers.</span><span class="sxs-lookup"><span data-stu-id="33b13-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="33b13-182">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="33b13-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="33b13-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="33b13-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="33b13-184">Int32</span><span class="sxs-lookup"><span data-stu-id="33b13-184">Int32</span></span>|<span data-ttu-id="33b13-185">Wert für den von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) geerbten Zertifikats Gültigkeitszeitraum</span><span class="sxs-lookup"><span data-stu-id="33b13-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="33b13-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="33b13-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="33b13-187">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="33b13-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="33b13-188">Skalierung für den von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)geerbten Zertifikats Gültigkeitszeitraum.</span><span class="sxs-lookup"><span data-stu-id="33b13-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="33b13-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="33b13-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="33b13-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="33b13-190">certificationAuthority</span></span>|<span data-ttu-id="33b13-191">String</span><span class="sxs-lookup"><span data-stu-id="33b13-191">String</span></span>|<span data-ttu-id="33b13-192">PKCS-ZertifizierungsStelle</span><span class="sxs-lookup"><span data-stu-id="33b13-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="33b13-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="33b13-193">certificationAuthorityName</span></span>|<span data-ttu-id="33b13-194">String</span><span class="sxs-lookup"><span data-stu-id="33b13-194">String</span></span>|<span data-ttu-id="33b13-195">Name der PKCS-ZertifizierungsStelle</span><span class="sxs-lookup"><span data-stu-id="33b13-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="33b13-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="33b13-196">certificateTemplateName</span></span>|<span data-ttu-id="33b13-197">String</span><span class="sxs-lookup"><span data-stu-id="33b13-197">String</span></span>|<span data-ttu-id="33b13-198">Name der PKCS-Zertifikatvorlage</span><span class="sxs-lookup"><span data-stu-id="33b13-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="33b13-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="33b13-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="33b13-200">String</span><span class="sxs-lookup"><span data-stu-id="33b13-200">String</span></span>|<span data-ttu-id="33b13-201">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="33b13-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="33b13-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="33b13-202">extendedKeyUsages</span></span>|<span data-ttu-id="33b13-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="33b13-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="33b13-204">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="33b13-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="33b13-205">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="33b13-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="33b13-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="33b13-206">Response</span></span>
<span data-ttu-id="33b13-207">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windows10pkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="33b13-207">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b13-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33b13-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="33b13-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33b13-209">Request</span></span>
<span data-ttu-id="33b13-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33b13-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="33b13-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="33b13-211">Response</span></span>
<span data-ttu-id="33b13-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33b13-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




