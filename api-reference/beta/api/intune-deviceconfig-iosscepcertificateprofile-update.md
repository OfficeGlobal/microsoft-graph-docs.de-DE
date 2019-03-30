---
title: Iosscepcertificateprofile hinzugefügt aktualisieren
description: Aktualisieren der Eigenschaften eines Iosscepcertificateprofile hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2416c3006e007d10bfa1489eb24c94d244261926
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986061"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="d4627-103">Iosscepcertificateprofile hinzugefügt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d4627-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="d4627-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4627-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4627-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d4627-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4627-106">Aktualisieren der Eigenschaften eines [iosscepcertificateprofile hinzugefügt](../resources/intune-deviceconfig-iosscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4627-106">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4627-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4627-107">Prerequisites</span></span>
<span data-ttu-id="d4627-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4627-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4627-110">Permission type</span></span>|<span data-ttu-id="d4627-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4627-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4627-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4627-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4627-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4627-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4627-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4627-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4627-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4627-115">Not supported.</span></span>|
|<span data-ttu-id="d4627-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4627-116">Application</span></span>|<span data-ttu-id="d4627-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4627-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4627-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4627-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4627-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4627-119">Request headers</span></span>
|<span data-ttu-id="d4627-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d4627-120">Header</span></span>|<span data-ttu-id="d4627-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d4627-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4627-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4627-122">Authorization</span></span>|<span data-ttu-id="d4627-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4627-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4627-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4627-124">Accept</span></span>|<span data-ttu-id="d4627-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4627-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4627-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4627-126">Request body</span></span>
<span data-ttu-id="d4627-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosscepcertificateprofile hinzugefügt](../resources/intune-deviceconfig-iosscepcertificateprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d4627-127">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="d4627-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosscepcertificateprofile hinzugefügt](../resources/intune-deviceconfig-iosscepcertificateprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d4627-128">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="d4627-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4627-129">Property</span></span>|<span data-ttu-id="d4627-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d4627-130">Type</span></span>|<span data-ttu-id="d4627-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4627-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4627-132">id</span><span class="sxs-lookup"><span data-stu-id="d4627-132">id</span></span>|<span data-ttu-id="d4627-133">String</span><span class="sxs-lookup"><span data-stu-id="d4627-133">String</span></span>|<span data-ttu-id="d4627-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d4627-134">Key of the entity.</span></span> <span data-ttu-id="d4627-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4627-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4627-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4627-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d4627-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4627-137">DateTimeOffset</span></span>|<span data-ttu-id="d4627-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4627-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d4627-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4627-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4627-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="d4627-140">roleScopeTagIds</span></span>|<span data-ttu-id="d4627-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d4627-141">String collection</span></span>|<span data-ttu-id="d4627-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="d4627-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4627-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4627-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4627-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d4627-144">supportsScopeTags</span></span>|<span data-ttu-id="d4627-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4627-145">Boolean</span></span>|<span data-ttu-id="d4627-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4627-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d4627-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="d4627-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d4627-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d4627-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d4627-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4627-149">This property is read-only.</span></span> <span data-ttu-id="d4627-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4627-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4627-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4627-151">createdDateTime</span></span>|<span data-ttu-id="d4627-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4627-152">DateTimeOffset</span></span>|<span data-ttu-id="d4627-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4627-153">DateTime the object was created.</span></span> <span data-ttu-id="d4627-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4627-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4627-155">description</span><span class="sxs-lookup"><span data-stu-id="d4627-155">description</span></span>|<span data-ttu-id="d4627-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4627-156">String</span></span>|<span data-ttu-id="d4627-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d4627-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4627-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4627-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4627-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d4627-159">displayName</span></span>|<span data-ttu-id="d4627-160">String</span><span class="sxs-lookup"><span data-stu-id="d4627-160">String</span></span>|<span data-ttu-id="d4627-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d4627-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4627-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4627-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4627-163">Version</span><span class="sxs-lookup"><span data-stu-id="d4627-163">version</span></span>|<span data-ttu-id="d4627-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d4627-164">Int32</span></span>|<span data-ttu-id="d4627-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d4627-165">Version of the device configuration.</span></span> <span data-ttu-id="d4627-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4627-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4627-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="d4627-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="d4627-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d4627-168">Int32</span></span>|<span data-ttu-id="d4627-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="d4627-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d4627-170">Gültige Werte 1 bis 99 geerbt von [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d4627-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d4627-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d4627-171">subjectNameFormat</span></span>|[<span data-ttu-id="d4627-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d4627-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="d4627-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="d4627-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="d4627-174">Von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="d4627-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="d4627-175">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="d4627-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="d4627-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d4627-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d4627-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d4627-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d4627-178">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="d4627-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="d4627-179">Von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="d4627-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="d4627-180">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="d4627-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d4627-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d4627-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d4627-182">Int32</span><span class="sxs-lookup"><span data-stu-id="d4627-182">Int32</span></span>|<span data-ttu-id="d4627-183">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="d4627-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d4627-184">Geerbt von [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d4627-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d4627-185">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="d4627-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d4627-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="d4627-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d4627-187">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="d4627-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d4627-188">Von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="d4627-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="d4627-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="d4627-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d4627-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="d4627-190">scepServerUrls</span></span>|<span data-ttu-id="d4627-191">String collection</span><span class="sxs-lookup"><span data-stu-id="d4627-191">String collection</span></span>|<span data-ttu-id="d4627-192">SCEP-Server-URL (s).</span><span class="sxs-lookup"><span data-stu-id="d4627-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="d4627-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d4627-193">subjectNameFormatString</span></span>|<span data-ttu-id="d4627-194">String</span><span class="sxs-lookup"><span data-stu-id="d4627-194">String</span></span>|<span data-ttu-id="d4627-195">Benutzerdefiniertes Format, das mit SubjectNameFormat = Custom verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d4627-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="d4627-196">Beispiel: CN = {{Email Adresse}}, E = {Email Adresse}}, OU = Enterprise users, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="d4627-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="d4627-197">keyUsage</span><span class="sxs-lookup"><span data-stu-id="d4627-197">keyUsage</span></span>|[<span data-ttu-id="d4627-198">keyUsages</span><span class="sxs-lookup"><span data-stu-id="d4627-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="d4627-199">SCEP-Schlüsselverwendung.</span><span class="sxs-lookup"><span data-stu-id="d4627-199">SCEP Key Usage.</span></span> <span data-ttu-id="d4627-200">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="d4627-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="d4627-201">keySize</span><span class="sxs-lookup"><span data-stu-id="d4627-201">keySize</span></span>|[<span data-ttu-id="d4627-202">keySize</span><span class="sxs-lookup"><span data-stu-id="d4627-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="d4627-203">SCEP-Schlüsselgröße.</span><span class="sxs-lookup"><span data-stu-id="d4627-203">SCEP Key Size.</span></span> <span data-ttu-id="d4627-204">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="d4627-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="d4627-205">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d4627-205">extendedKeyUsages</span></span>|<span data-ttu-id="d4627-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d4627-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d4627-207">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="d4627-207">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d4627-208">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d4627-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d4627-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d4627-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d4627-210">String</span><span class="sxs-lookup"><span data-stu-id="d4627-210">String</span></span>|<span data-ttu-id="d4627-211">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="d4627-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="d4627-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d4627-212">certificateStore</span></span>|[<span data-ttu-id="d4627-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d4627-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="d4627-214">Zielspeicher Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="d4627-214">Target store certificate.</span></span> <span data-ttu-id="d4627-215">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="d4627-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="d4627-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="d4627-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="d4627-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d4627-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="d4627-218">Benutzerdefinierte Alterantive.</span><span class="sxs-lookup"><span data-stu-id="d4627-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="d4627-219">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d4627-219">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d4627-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4627-220">Response</span></span>
<span data-ttu-id="d4627-221">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosscepcertificateprofile hinzugefügt](../resources/intune-deviceconfig-iosscepcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d4627-221">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4627-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4627-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4627-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4627-223">Request</span></span>
<span data-ttu-id="d4627-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4627-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d4627-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4627-225">Response</span></span>
<span data-ttu-id="d4627-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4627-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```




