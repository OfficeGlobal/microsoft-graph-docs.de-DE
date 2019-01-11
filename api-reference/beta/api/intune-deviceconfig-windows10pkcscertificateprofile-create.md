---
title: Erstellen von windows10PkcsCertificateProfile
description: Erstellen eines neuen windows10PkcsCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d93477adb0358196f0bfa2bedd8ef35a555ee7e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809274"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="45cd0-103">Erstellen von windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="45cd0-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="45cd0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="45cd0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45cd0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="45cd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45cd0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="45cd0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45cd0-107">Erstellen eines neuen [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="45cd0-107">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45cd0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="45cd0-108">Prerequisites</span></span>
<span data-ttu-id="45cd0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45cd0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45cd0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45cd0-111">Permission type</span></span>|<span data-ttu-id="45cd0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45cd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45cd0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45cd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45cd0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45cd0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45cd0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45cd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45cd0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45cd0-116">Not supported.</span></span>|
|<span data-ttu-id="45cd0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45cd0-117">Application</span></span>|<span data-ttu-id="45cd0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45cd0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45cd0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45cd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45cd0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45cd0-120">Request headers</span></span>
|<span data-ttu-id="45cd0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="45cd0-121">Header</span></span>|<span data-ttu-id="45cd0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="45cd0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45cd0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45cd0-123">Authorization</span></span>|<span data-ttu-id="45cd0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="45cd0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45cd0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="45cd0-125">Accept</span></span>|<span data-ttu-id="45cd0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45cd0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45cd0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45cd0-127">Request body</span></span>
<span data-ttu-id="45cd0-128">Geben Sie im Textkörper Anforderung für das Objekt windows10PkcsCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="45cd0-128">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="45cd0-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows10PkcsCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="45cd0-129">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="45cd0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45cd0-130">Property</span></span>|<span data-ttu-id="45cd0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="45cd0-131">Type</span></span>|<span data-ttu-id="45cd0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45cd0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45cd0-133">id</span><span class="sxs-lookup"><span data-stu-id="45cd0-133">id</span></span>|<span data-ttu-id="45cd0-134">String</span><span class="sxs-lookup"><span data-stu-id="45cd0-134">String</span></span>|<span data-ttu-id="45cd0-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="45cd0-135">Key of the entity.</span></span> <span data-ttu-id="45cd0-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45cd0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="45cd0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45cd0-138">DateTimeOffset</span></span>|<span data-ttu-id="45cd0-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="45cd0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="45cd0-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45cd0-141">roleScopeTagIds</span></span>|<span data-ttu-id="45cd0-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="45cd0-142">String collection</span></span>|<span data-ttu-id="45cd0-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="45cd0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="45cd0-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="45cd0-145">supportsScopeTags</span></span>|<span data-ttu-id="45cd0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="45cd0-146">Boolean</span></span>|<span data-ttu-id="45cd0-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="45cd0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45cd0-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="45cd0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45cd0-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="45cd0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45cd0-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="45cd0-150">This property is read-only.</span></span> <span data-ttu-id="45cd0-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45cd0-152">createdDateTime</span></span>|<span data-ttu-id="45cd0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45cd0-153">DateTimeOffset</span></span>|<span data-ttu-id="45cd0-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="45cd0-154">DateTime the object was created.</span></span> <span data-ttu-id="45cd0-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd0-156">description</span><span class="sxs-lookup"><span data-stu-id="45cd0-156">description</span></span>|<span data-ttu-id="45cd0-157">String</span><span class="sxs-lookup"><span data-stu-id="45cd0-157">String</span></span>|<span data-ttu-id="45cd0-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="45cd0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45cd0-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="45cd0-160">displayName</span></span>|<span data-ttu-id="45cd0-161">String</span><span class="sxs-lookup"><span data-stu-id="45cd0-161">String</span></span>|<span data-ttu-id="45cd0-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="45cd0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45cd0-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd0-164">Version</span><span class="sxs-lookup"><span data-stu-id="45cd0-164">version</span></span>|<span data-ttu-id="45cd0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="45cd0-165">Int32</span></span>|<span data-ttu-id="45cd0-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="45cd0-166">Version of the device configuration.</span></span> <span data-ttu-id="45cd0-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd0-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="45cd0-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="45cd0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="45cd0-169">Int32</span></span>|<span data-ttu-id="45cd0-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="45cd0-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="45cd0-171">Gültige Werte 1 bis 99 Inherited aus [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45cd0-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="45cd0-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="45cd0-172">keyStorageProvider</span></span>|[<span data-ttu-id="45cd0-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="45cd0-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="45cd0-174">Schlüssel-Speicher-Anbieter (KSP) Inherited aus [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="45cd0-175">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="45cd0-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="45cd0-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="45cd0-176">subjectNameFormat</span></span>|[<span data-ttu-id="45cd0-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="45cd0-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="45cd0-178">Zertifikat Subject Name Format geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="45cd0-179">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="45cd0-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="45cd0-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="45cd0-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="45cd0-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="45cd0-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="45cd0-182">Zertifikat Subject Alternative Name Typ geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="45cd0-183">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="45cd0-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="45cd0-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="45cd0-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="45cd0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="45cd0-185">Int32</span></span>|<span data-ttu-id="45cd0-186">Wert für das Zertifikat Gültigkeit Zeitraum geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45cd0-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="45cd0-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="45cd0-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="45cd0-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="45cd0-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="45cd0-189">Skalierung für das Zertifikat Gültigkeit Zeitraum geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45cd0-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="45cd0-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="45cd0-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="45cd0-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="45cd0-191">certificationAuthority</span></span>|<span data-ttu-id="45cd0-192">String</span><span class="sxs-lookup"><span data-stu-id="45cd0-192">String</span></span>|<span data-ttu-id="45cd0-193">PKCS-Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="45cd0-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="45cd0-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="45cd0-194">certificationAuthorityName</span></span>|<span data-ttu-id="45cd0-195">String</span><span class="sxs-lookup"><span data-stu-id="45cd0-195">String</span></span>|<span data-ttu-id="45cd0-196">Name der Zertifizierungsstelle PKCS</span><span class="sxs-lookup"><span data-stu-id="45cd0-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="45cd0-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="45cd0-197">certificateTemplateName</span></span>|<span data-ttu-id="45cd0-198">String</span><span class="sxs-lookup"><span data-stu-id="45cd0-198">String</span></span>|<span data-ttu-id="45cd0-199">Name der PKCS Zertifikatsvorlage</span><span class="sxs-lookup"><span data-stu-id="45cd0-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="45cd0-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="45cd0-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="45cd0-201">String</span><span class="sxs-lookup"><span data-stu-id="45cd0-201">String</span></span>|<span data-ttu-id="45cd0-202">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="45cd0-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="45cd0-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="45cd0-203">extendedKeyUsages</span></span>|<span data-ttu-id="45cd0-204">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="45cd0-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="45cd0-205">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="45cd0-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="45cd0-206">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="45cd0-206">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="45cd0-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="45cd0-207">Response</span></span>
<span data-ttu-id="45cd0-208">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="45cd0-208">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45cd0-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45cd0-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="45cd0-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45cd0-210">Request</span></span>
<span data-ttu-id="45cd0-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45cd0-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="45cd0-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="45cd0-212">Response</span></span>
<span data-ttu-id="45cd0-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45cd0-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





