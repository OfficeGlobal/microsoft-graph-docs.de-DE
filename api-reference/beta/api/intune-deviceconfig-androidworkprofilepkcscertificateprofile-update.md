---
title: AndroidWorkProfilePkcsCertificateProfile aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfilePkcsCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fbba0e2ae5974d9cd0738a5079c5c1324f00cfe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154495"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="d88ab-103">AndroidWorkProfilePkcsCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d88ab-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="d88ab-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d88ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d88ab-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d88ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d88ab-106">Aktualisieren der Eigenschaften eines [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d88ab-106">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d88ab-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d88ab-107">Prerequisites</span></span>
<span data-ttu-id="d88ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d88ab-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d88ab-110">Permission type</span></span>|<span data-ttu-id="d88ab-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d88ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d88ab-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d88ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d88ab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d88ab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d88ab-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d88ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d88ab-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d88ab-115">Not supported.</span></span>|
|<span data-ttu-id="d88ab-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d88ab-116">Application</span></span>|<span data-ttu-id="d88ab-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d88ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d88ab-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d88ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d88ab-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d88ab-119">Request headers</span></span>
|<span data-ttu-id="d88ab-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d88ab-120">Header</span></span>|<span data-ttu-id="d88ab-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d88ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d88ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d88ab-122">Authorization</span></span>|<span data-ttu-id="d88ab-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d88ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d88ab-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d88ab-124">Accept</span></span>|<span data-ttu-id="d88ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d88ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d88ab-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d88ab-126">Request body</span></span>
<span data-ttu-id="d88ab-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d88ab-127">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="d88ab-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d88ab-128">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="d88ab-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d88ab-129">Property</span></span>|<span data-ttu-id="d88ab-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d88ab-130">Type</span></span>|<span data-ttu-id="d88ab-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d88ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d88ab-132">id</span><span class="sxs-lookup"><span data-stu-id="d88ab-132">id</span></span>|<span data-ttu-id="d88ab-133">string</span><span class="sxs-lookup"><span data-stu-id="d88ab-133">String</span></span>|<span data-ttu-id="d88ab-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d88ab-134">Key of the entity.</span></span> <span data-ttu-id="d88ab-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d88ab-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d88ab-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d88ab-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d88ab-137">DateTimeOffset</span></span>|<span data-ttu-id="d88ab-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d88ab-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d88ab-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d88ab-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="d88ab-140">roleScopeTagIds</span></span>|<span data-ttu-id="d88ab-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d88ab-141">String collection</span></span>|<span data-ttu-id="d88ab-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="d88ab-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d88ab-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d88ab-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d88ab-144">supportsScopeTags</span></span>|<span data-ttu-id="d88ab-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d88ab-145">Boolean</span></span>|<span data-ttu-id="d88ab-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d88ab-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d88ab-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="d88ab-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d88ab-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d88ab-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d88ab-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d88ab-149">This property is read-only.</span></span> <span data-ttu-id="d88ab-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d88ab-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d88ab-151">createdDateTime</span></span>|<span data-ttu-id="d88ab-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d88ab-152">DateTimeOffset</span></span>|<span data-ttu-id="d88ab-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d88ab-153">DateTime the object was created.</span></span> <span data-ttu-id="d88ab-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d88ab-155">description</span><span class="sxs-lookup"><span data-stu-id="d88ab-155">description</span></span>|<span data-ttu-id="d88ab-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d88ab-156">String</span></span>|<span data-ttu-id="d88ab-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d88ab-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d88ab-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d88ab-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d88ab-159">displayName</span></span>|<span data-ttu-id="d88ab-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d88ab-160">String</span></span>|<span data-ttu-id="d88ab-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d88ab-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d88ab-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d88ab-163">Version</span><span class="sxs-lookup"><span data-stu-id="d88ab-163">version</span></span>|<span data-ttu-id="d88ab-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d88ab-164">Int32</span></span>|<span data-ttu-id="d88ab-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d88ab-165">Version of the device configuration.</span></span> <span data-ttu-id="d88ab-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d88ab-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d88ab-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="d88ab-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="d88ab-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d88ab-168">Int32</span></span>|<span data-ttu-id="d88ab-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="d88ab-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d88ab-170">Gültige Werte 1 bis 99 geerbt von [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d88ab-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d88ab-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d88ab-171">subjectNameFormat</span></span>|[<span data-ttu-id="d88ab-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d88ab-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d88ab-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="d88ab-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="d88ab-174">Von [AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="d88ab-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="d88ab-175">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="d88ab-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d88ab-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d88ab-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d88ab-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d88ab-177">Int32</span></span>|<span data-ttu-id="d88ab-178">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="d88ab-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d88ab-179">Geerbt von [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d88ab-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d88ab-180">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="d88ab-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d88ab-181">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="d88ab-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d88ab-182">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="d88ab-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d88ab-183">Von [AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="d88ab-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="d88ab-184">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="d88ab-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d88ab-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d88ab-185">extendedKeyUsages</span></span>|<span data-ttu-id="d88ab-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d88ab-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d88ab-187">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="d88ab-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d88ab-188">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d88ab-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d88ab-189">Geerbt von [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d88ab-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d88ab-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="d88ab-190">certificationAuthority</span></span>|<span data-ttu-id="d88ab-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d88ab-191">String</span></span>|<span data-ttu-id="d88ab-192">PKCS-ZertifizierungsStelle</span><span class="sxs-lookup"><span data-stu-id="d88ab-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="d88ab-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="d88ab-193">certificationAuthorityName</span></span>|<span data-ttu-id="d88ab-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d88ab-194">String</span></span>|<span data-ttu-id="d88ab-195">Name der PKCS-ZertifizierungsStelle</span><span class="sxs-lookup"><span data-stu-id="d88ab-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="d88ab-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="d88ab-196">certificateTemplateName</span></span>|<span data-ttu-id="d88ab-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d88ab-197">String</span></span>|<span data-ttu-id="d88ab-198">Name der PKCS-Zertifikatvorlage</span><span class="sxs-lookup"><span data-stu-id="d88ab-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="d88ab-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d88ab-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d88ab-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d88ab-200">String</span></span>|<span data-ttu-id="d88ab-201">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="d88ab-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="d88ab-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d88ab-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d88ab-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d88ab-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d88ab-204">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="d88ab-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d88ab-205">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="d88ab-205">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="d88ab-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="d88ab-206">Response</span></span>
<span data-ttu-id="d88ab-207">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d88ab-207">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d88ab-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d88ab-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="d88ab-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d88ab-209">Request</span></span>
<span data-ttu-id="d88ab-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d88ab-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 969

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="d88ab-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="d88ab-211">Response</span></span>
<span data-ttu-id="d88ab-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d88ab-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




