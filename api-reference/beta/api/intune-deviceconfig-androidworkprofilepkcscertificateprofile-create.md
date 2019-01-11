---
title: Erstellen von androidWorkProfilePkcsCertificateProfile
description: Erstellen eines neuen AndroidWorkProfilePkcsCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 781b6f53d5530d68c19fb205f5c8f55b44bc0588
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849098"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="5f4bc-103">Erstellen von androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5f4bc-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="5f4bc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f4bc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f4bc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f4bc-107">Erstellen eines neuen [AndroidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-107">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f4bc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f4bc-108">Prerequisites</span></span>
<span data-ttu-id="5f4bc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f4bc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f4bc-111">Permission type</span></span>|<span data-ttu-id="5f4bc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f4bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f4bc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f4bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f4bc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f4bc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f4bc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f4bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f4bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f4bc-116">Not supported.</span></span>|
|<span data-ttu-id="5f4bc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f4bc-117">Application</span></span>|<span data-ttu-id="5f4bc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f4bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f4bc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f4bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5f4bc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f4bc-120">Request headers</span></span>
|<span data-ttu-id="5f4bc-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5f4bc-121">Header</span></span>|<span data-ttu-id="5f4bc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5f4bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f4bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f4bc-123">Authorization</span></span>|<span data-ttu-id="5f4bc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f4bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f4bc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5f4bc-125">Accept</span></span>|<span data-ttu-id="5f4bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f4bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f4bc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f4bc-127">Request body</span></span>
<span data-ttu-id="5f4bc-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfilePkcsCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-128">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="5f4bc-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfilePkcsCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-129">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="5f4bc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f4bc-130">Property</span></span>|<span data-ttu-id="5f4bc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5f4bc-131">Type</span></span>|<span data-ttu-id="5f4bc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f4bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f4bc-133">id</span><span class="sxs-lookup"><span data-stu-id="5f4bc-133">id</span></span>|<span data-ttu-id="5f4bc-134">String</span><span class="sxs-lookup"><span data-stu-id="5f4bc-134">String</span></span>|<span data-ttu-id="5f4bc-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5f4bc-135">Key of the entity.</span></span> <span data-ttu-id="5f4bc-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f4bc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f4bc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5f4bc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f4bc-138">DateTimeOffset</span></span>|<span data-ttu-id="5f4bc-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5f4bc-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f4bc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5f4bc-141">roleScopeTagIds</span></span>|<span data-ttu-id="5f4bc-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="5f4bc-142">String collection</span></span>|<span data-ttu-id="5f4bc-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5f4bc-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f4bc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5f4bc-145">supportsScopeTags</span></span>|<span data-ttu-id="5f4bc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f4bc-146">Boolean</span></span>|<span data-ttu-id="5f4bc-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5f4bc-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5f4bc-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5f4bc-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-150">This property is read-only.</span></span> <span data-ttu-id="5f4bc-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f4bc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f4bc-152">createdDateTime</span></span>|<span data-ttu-id="5f4bc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f4bc-153">DateTimeOffset</span></span>|<span data-ttu-id="5f4bc-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-154">DateTime the object was created.</span></span> <span data-ttu-id="5f4bc-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f4bc-156">description</span><span class="sxs-lookup"><span data-stu-id="5f4bc-156">description</span></span>|<span data-ttu-id="5f4bc-157">String</span><span class="sxs-lookup"><span data-stu-id="5f4bc-157">String</span></span>|<span data-ttu-id="5f4bc-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5f4bc-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f4bc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5f4bc-160">displayName</span></span>|<span data-ttu-id="5f4bc-161">String</span><span class="sxs-lookup"><span data-stu-id="5f4bc-161">String</span></span>|<span data-ttu-id="5f4bc-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5f4bc-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f4bc-164">Version</span><span class="sxs-lookup"><span data-stu-id="5f4bc-164">version</span></span>|<span data-ttu-id="5f4bc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5f4bc-165">Int32</span></span>|<span data-ttu-id="5f4bc-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-166">Version of the device configuration.</span></span> <span data-ttu-id="5f4bc-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f4bc-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5f4bc-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="5f4bc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="5f4bc-169">Int32</span></span>|<span data-ttu-id="5f4bc-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5f4bc-171">Gültige Werte 1 bis 99 Inherited aus [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5f4bc-171">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5f4bc-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5f4bc-172">subjectNameFormat</span></span>|[<span data-ttu-id="5f4bc-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5f4bc-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="5f4bc-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="5f4bc-175">Geerbt von [AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-175">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="5f4bc-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="5f4bc-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5f4bc-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5f4bc-178">Int32</span><span class="sxs-lookup"><span data-stu-id="5f4bc-178">Int32</span></span>|<span data-ttu-id="5f4bc-179">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5f4bc-180">Geerbt von [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5f4bc-180">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5f4bc-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5f4bc-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5f4bc-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5f4bc-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5f4bc-183">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5f4bc-184">Geerbt von [AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5f4bc-184">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="5f4bc-185">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5f4bc-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="5f4bc-186">extendedKeyUsages</span></span>|<span data-ttu-id="5f4bc-187">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5f4bc-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="5f4bc-188">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="5f4bc-189">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5f4bc-190">Geerbt von [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5f4bc-190">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5f4bc-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="5f4bc-191">certificationAuthority</span></span>|<span data-ttu-id="5f4bc-192">String</span><span class="sxs-lookup"><span data-stu-id="5f4bc-192">String</span></span>|<span data-ttu-id="5f4bc-193">PKCS-Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="5f4bc-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="5f4bc-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="5f4bc-194">certificationAuthorityName</span></span>|<span data-ttu-id="5f4bc-195">String</span><span class="sxs-lookup"><span data-stu-id="5f4bc-195">String</span></span>|<span data-ttu-id="5f4bc-196">Name der Zertifizierungsstelle PKCS</span><span class="sxs-lookup"><span data-stu-id="5f4bc-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="5f4bc-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="5f4bc-197">certificateTemplateName</span></span>|<span data-ttu-id="5f4bc-198">String</span><span class="sxs-lookup"><span data-stu-id="5f4bc-198">String</span></span>|<span data-ttu-id="5f4bc-199">Name der PKCS Zertifikatsvorlage</span><span class="sxs-lookup"><span data-stu-id="5f4bc-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="5f4bc-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5f4bc-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5f4bc-201">String</span><span class="sxs-lookup"><span data-stu-id="5f4bc-201">String</span></span>|<span data-ttu-id="5f4bc-202">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="5f4bc-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5f4bc-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5f4bc-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5f4bc-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5f4bc-205">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="5f4bc-206">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="5f4bc-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f4bc-207">Response</span></span>
<span data-ttu-id="5f4bc-208">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f4bc-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f4bc-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f4bc-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f4bc-210">Request</span></span>
<span data-ttu-id="5f4bc-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1033

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="5f4bc-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f4bc-212">Response</span></span>
<span data-ttu-id="5f4bc-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f4bc-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1141

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```





