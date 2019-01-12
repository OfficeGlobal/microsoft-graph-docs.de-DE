---
title: Erstellen von windows10PkcsCertificateProfile
description: Erstellen eines neuen windows10PkcsCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85fd8c3dc8c8f1f8d00cf6b84cb342dc6172ee8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966755"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="6f0a2-103">Erstellen von windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6f0a2-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="6f0a2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f0a2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f0a2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f0a2-107">Erstellen eines neuen [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-107">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f0a2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f0a2-108">Prerequisites</span></span>
<span data-ttu-id="6f0a2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f0a2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f0a2-111">Permission type</span></span>|<span data-ttu-id="6f0a2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f0a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f0a2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f0a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f0a2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f0a2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f0a2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f0a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f0a2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f0a2-116">Not supported.</span></span>|
|<span data-ttu-id="6f0a2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f0a2-117">Application</span></span>|<span data-ttu-id="6f0a2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f0a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f0a2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f0a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6f0a2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f0a2-120">Request headers</span></span>
|<span data-ttu-id="6f0a2-121">Header</span><span class="sxs-lookup"><span data-stu-id="6f0a2-121">Header</span></span>|<span data-ttu-id="6f0a2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6f0a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f0a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f0a2-123">Authorization</span></span>|<span data-ttu-id="6f0a2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f0a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f0a2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6f0a2-125">Accept</span></span>|<span data-ttu-id="6f0a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f0a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f0a2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f0a2-127">Request body</span></span>
<span data-ttu-id="6f0a2-128">Geben Sie im Textkörper Anforderung für das Objekt windows10PkcsCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-128">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="6f0a2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows10PkcsCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-129">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="6f0a2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f0a2-130">Property</span></span>|<span data-ttu-id="6f0a2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6f0a2-131">Type</span></span>|<span data-ttu-id="6f0a2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f0a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f0a2-133">id</span><span class="sxs-lookup"><span data-stu-id="6f0a2-133">id</span></span>|<span data-ttu-id="6f0a2-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f0a2-134">String</span></span>|<span data-ttu-id="6f0a2-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6f0a2-135">Key of the entity.</span></span> <span data-ttu-id="6f0a2-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0a2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f0a2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f0a2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f0a2-138">DateTimeOffset</span></span>|<span data-ttu-id="6f0a2-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6f0a2-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0a2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f0a2-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f0a2-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6f0a2-142">String collection</span></span>|<span data-ttu-id="6f0a2-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f0a2-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0a2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f0a2-145">supportsScopeTags</span></span>|<span data-ttu-id="6f0a2-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6f0a2-146">Boolean</span></span>|<span data-ttu-id="6f0a2-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f0a2-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f0a2-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f0a2-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-150">This property is read-only.</span></span> <span data-ttu-id="6f0a2-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0a2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f0a2-152">createdDateTime</span></span>|<span data-ttu-id="6f0a2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f0a2-153">DateTimeOffset</span></span>|<span data-ttu-id="6f0a2-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-154">DateTime the object was created.</span></span> <span data-ttu-id="6f0a2-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0a2-156">description</span><span class="sxs-lookup"><span data-stu-id="6f0a2-156">description</span></span>|<span data-ttu-id="6f0a2-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f0a2-157">String</span></span>|<span data-ttu-id="6f0a2-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f0a2-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0a2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6f0a2-160">displayName</span></span>|<span data-ttu-id="6f0a2-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f0a2-161">String</span></span>|<span data-ttu-id="6f0a2-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f0a2-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0a2-164">Version</span><span class="sxs-lookup"><span data-stu-id="6f0a2-164">version</span></span>|<span data-ttu-id="6f0a2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0a2-165">Int32</span></span>|<span data-ttu-id="6f0a2-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-166">Version of the device configuration.</span></span> <span data-ttu-id="6f0a2-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0a2-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6f0a2-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="6f0a2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0a2-169">Int32</span></span>|<span data-ttu-id="6f0a2-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6f0a2-171">Gültige Werte 1 bis 99 Inherited aus [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6f0a2-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6f0a2-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="6f0a2-172">keyStorageProvider</span></span>|[<span data-ttu-id="6f0a2-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="6f0a2-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="6f0a2-174">Schlüssel-Speicher-Anbieter (KSP) Inherited aus [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6f0a2-175">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="6f0a2-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6f0a2-176">subjectNameFormat</span></span>|[<span data-ttu-id="6f0a2-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6f0a2-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6f0a2-178">Zertifikat Subject Name Format geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6f0a2-179">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6f0a2-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6f0a2-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6f0a2-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6f0a2-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6f0a2-182">Zertifikat Subject Alternative Name Typ geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6f0a2-183">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="6f0a2-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6f0a2-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6f0a2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0a2-185">Int32</span></span>|<span data-ttu-id="6f0a2-186">Wert für das Zertifikat Gültigkeit Zeitraum geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6f0a2-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6f0a2-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6f0a2-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6f0a2-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6f0a2-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6f0a2-189">Skalierung für das Zertifikat Gültigkeit Zeitraum geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f0a2-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6f0a2-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6f0a2-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="6f0a2-191">certificationAuthority</span></span>|<span data-ttu-id="6f0a2-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f0a2-192">String</span></span>|<span data-ttu-id="6f0a2-193">PKCS-Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="6f0a2-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="6f0a2-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="6f0a2-194">certificationAuthorityName</span></span>|<span data-ttu-id="6f0a2-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f0a2-195">String</span></span>|<span data-ttu-id="6f0a2-196">Name der Zertifizierungsstelle PKCS</span><span class="sxs-lookup"><span data-stu-id="6f0a2-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="6f0a2-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="6f0a2-197">certificateTemplateName</span></span>|<span data-ttu-id="6f0a2-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f0a2-198">String</span></span>|<span data-ttu-id="6f0a2-199">Name der PKCS Zertifikatsvorlage</span><span class="sxs-lookup"><span data-stu-id="6f0a2-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="6f0a2-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6f0a2-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="6f0a2-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f0a2-201">String</span></span>|<span data-ttu-id="6f0a2-202">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="6f0a2-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6f0a2-203">extendedKeyUsages</span></span>|<span data-ttu-id="6f0a2-204">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6f0a2-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="6f0a2-205">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="6f0a2-206">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-206">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6f0a2-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f0a2-207">Response</span></span>
<span data-ttu-id="6f0a2-208">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-208">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f0a2-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f0a2-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f0a2-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f0a2-210">Request</span></span>
<span data-ttu-id="6f0a2-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f0a2-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f0a2-212">Response</span></span>
<span data-ttu-id="6f0a2-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f0a2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





