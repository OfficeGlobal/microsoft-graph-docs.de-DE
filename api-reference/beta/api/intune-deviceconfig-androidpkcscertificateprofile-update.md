---
title: AndroidPkcsCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidPkcsCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4be9510a78bf5147455b434efd98b3804823e4ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807844"
---
# <a name="update-androidpkcscertificateprofile"></a><span data-ttu-id="b403c-103">AndroidPkcsCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b403c-103">Update androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="b403c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b403c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b403c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b403c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b403c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b403c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b403c-107">Aktualisieren Sie die Eigenschaften eines [AndroidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b403c-107">Update the properties of a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b403c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b403c-108">Prerequisites</span></span>
<span data-ttu-id="b403c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b403c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b403c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b403c-111">Permission type</span></span>|<span data-ttu-id="b403c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b403c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b403c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b403c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b403c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b403c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b403c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b403c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b403c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b403c-116">Not supported.</span></span>|
|<span data-ttu-id="b403c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b403c-117">Application</span></span>|<span data-ttu-id="b403c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b403c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b403c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b403c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b403c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b403c-120">Request headers</span></span>
|<span data-ttu-id="b403c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b403c-121">Header</span></span>|<span data-ttu-id="b403c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b403c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b403c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b403c-123">Authorization</span></span>|<span data-ttu-id="b403c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b403c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b403c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b403c-125">Accept</span></span>|<span data-ttu-id="b403c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b403c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b403c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b403c-127">Request body</span></span>
<span data-ttu-id="b403c-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b403c-128">In the request body, supply a JSON representation for the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="b403c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b403c-129">The following table shows the properties that are required when you create the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="b403c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b403c-130">Property</span></span>|<span data-ttu-id="b403c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b403c-131">Type</span></span>|<span data-ttu-id="b403c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b403c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b403c-133">id</span><span class="sxs-lookup"><span data-stu-id="b403c-133">id</span></span>|<span data-ttu-id="b403c-134">String</span><span class="sxs-lookup"><span data-stu-id="b403c-134">String</span></span>|<span data-ttu-id="b403c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b403c-135">Key of the entity.</span></span> <span data-ttu-id="b403c-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b403c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b403c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b403c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b403c-138">DateTimeOffset</span></span>|<span data-ttu-id="b403c-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b403c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b403c-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b403c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b403c-141">roleScopeTagIds</span></span>|<span data-ttu-id="b403c-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b403c-142">String collection</span></span>|<span data-ttu-id="b403c-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b403c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b403c-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b403c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b403c-145">supportsScopeTags</span></span>|<span data-ttu-id="b403c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b403c-146">Boolean</span></span>|<span data-ttu-id="b403c-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b403c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b403c-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b403c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b403c-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b403c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b403c-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b403c-150">This property is read-only.</span></span> <span data-ttu-id="b403c-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b403c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b403c-152">createdDateTime</span></span>|<span data-ttu-id="b403c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b403c-153">DateTimeOffset</span></span>|<span data-ttu-id="b403c-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b403c-154">DateTime the object was created.</span></span> <span data-ttu-id="b403c-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b403c-156">description</span><span class="sxs-lookup"><span data-stu-id="b403c-156">description</span></span>|<span data-ttu-id="b403c-157">String</span><span class="sxs-lookup"><span data-stu-id="b403c-157">String</span></span>|<span data-ttu-id="b403c-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b403c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b403c-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b403c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b403c-160">displayName</span></span>|<span data-ttu-id="b403c-161">String</span><span class="sxs-lookup"><span data-stu-id="b403c-161">String</span></span>|<span data-ttu-id="b403c-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b403c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b403c-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b403c-164">Version</span><span class="sxs-lookup"><span data-stu-id="b403c-164">version</span></span>|<span data-ttu-id="b403c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b403c-165">Int32</span></span>|<span data-ttu-id="b403c-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b403c-166">Version of the device configuration.</span></span> <span data-ttu-id="b403c-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b403c-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b403c-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b403c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b403c-169">Int32</span></span>|<span data-ttu-id="b403c-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="b403c-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b403c-171">Gültige Werte 1 bis 99 Inherited aus [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b403c-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b403c-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b403c-172">subjectNameFormat</span></span>|[<span data-ttu-id="b403c-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b403c-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b403c-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="b403c-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="b403c-175">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b403c-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b403c-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b403c-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b403c-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b403c-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b403c-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b403c-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="b403c-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b403c-180">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b403c-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b403c-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b403c-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b403c-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b403c-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b403c-183">Int32</span></span>|<span data-ttu-id="b403c-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="b403c-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b403c-185">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b403c-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b403c-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b403c-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b403c-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b403c-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b403c-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="b403c-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b403c-189">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b403c-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b403c-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="b403c-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b403c-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b403c-191">extendedKeyUsages</span></span>|<span data-ttu-id="b403c-192">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b403c-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b403c-193">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="b403c-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b403c-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b403c-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b403c-195">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b403c-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b403c-196">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="b403c-196">certificationAuthority</span></span>|<span data-ttu-id="b403c-197">String</span><span class="sxs-lookup"><span data-stu-id="b403c-197">String</span></span>|<span data-ttu-id="b403c-198">PKCS-Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="b403c-198">PKCS Certification Authority</span></span>|
|<span data-ttu-id="b403c-199">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="b403c-199">certificationAuthorityName</span></span>|<span data-ttu-id="b403c-200">String</span><span class="sxs-lookup"><span data-stu-id="b403c-200">String</span></span>|<span data-ttu-id="b403c-201">Name der Zertifizierungsstelle PKCS</span><span class="sxs-lookup"><span data-stu-id="b403c-201">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="b403c-202">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="b403c-202">certificateTemplateName</span></span>|<span data-ttu-id="b403c-203">String</span><span class="sxs-lookup"><span data-stu-id="b403c-203">String</span></span>|<span data-ttu-id="b403c-204">Name der PKCS Zertifikatsvorlage</span><span class="sxs-lookup"><span data-stu-id="b403c-204">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="b403c-205">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b403c-205">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b403c-206">String</span><span class="sxs-lookup"><span data-stu-id="b403c-206">String</span></span>|<span data-ttu-id="b403c-207">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="b403c-207">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="b403c-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="b403c-208">Response</span></span>
<span data-ttu-id="b403c-209">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b403c-209">If successful, this method returns a `200 OK` response code and an updated [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b403c-210">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b403c-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="b403c-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b403c-211">Request</span></span>
<span data-ttu-id="b403c-212">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b403c-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 954

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
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="b403c-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="b403c-213">Response</span></span>
<span data-ttu-id="b403c-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b403c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





