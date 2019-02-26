---
title: AndroidWorkProfileScepCertificateProfile aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileScepCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5cf2180a4112b22398080e61ce4aa182d1865a3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143330"
---
# <a name="update-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="62e91-103">AndroidWorkProfileScepCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="62e91-103">Update androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="62e91-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62e91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62e91-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="62e91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62e91-106">Aktualisieren der Eigenschaften eines [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="62e91-106">Update the properties of a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62e91-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="62e91-107">Prerequisites</span></span>
<span data-ttu-id="62e91-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62e91-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62e91-110">Permission type</span></span>|<span data-ttu-id="62e91-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62e91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62e91-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62e91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62e91-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62e91-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62e91-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62e91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62e91-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62e91-115">Not supported.</span></span>|
|<span data-ttu-id="62e91-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62e91-116">Application</span></span>|<span data-ttu-id="62e91-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62e91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62e91-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62e91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="62e91-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62e91-119">Request headers</span></span>
|<span data-ttu-id="62e91-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="62e91-120">Header</span></span>|<span data-ttu-id="62e91-121">Wert</span><span class="sxs-lookup"><span data-stu-id="62e91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62e91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62e91-122">Authorization</span></span>|<span data-ttu-id="62e91-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="62e91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62e91-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="62e91-124">Accept</span></span>|<span data-ttu-id="62e91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62e91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62e91-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62e91-126">Request body</span></span>
<span data-ttu-id="62e91-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="62e91-127">In the request body, supply a JSON representation for the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

<span data-ttu-id="62e91-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="62e91-128">The following table shows the properties that are required when you create the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span></span>

|<span data-ttu-id="62e91-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62e91-129">Property</span></span>|<span data-ttu-id="62e91-130">Typ</span><span class="sxs-lookup"><span data-stu-id="62e91-130">Type</span></span>|<span data-ttu-id="62e91-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62e91-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62e91-132">id</span><span class="sxs-lookup"><span data-stu-id="62e91-132">id</span></span>|<span data-ttu-id="62e91-133">string</span><span class="sxs-lookup"><span data-stu-id="62e91-133">String</span></span>|<span data-ttu-id="62e91-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="62e91-134">Key of the entity.</span></span> <span data-ttu-id="62e91-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62e91-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62e91-136">lastModifiedDateTime</span></span>|<span data-ttu-id="62e91-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62e91-137">DateTimeOffset</span></span>|<span data-ttu-id="62e91-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="62e91-138">DateTime the object was last modified.</span></span> <span data-ttu-id="62e91-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62e91-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="62e91-140">roleScopeTagIds</span></span>|<span data-ttu-id="62e91-141">String collection</span><span class="sxs-lookup"><span data-stu-id="62e91-141">String collection</span></span>|<span data-ttu-id="62e91-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="62e91-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62e91-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62e91-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62e91-144">supportsScopeTags</span></span>|<span data-ttu-id="62e91-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="62e91-145">Boolean</span></span>|<span data-ttu-id="62e91-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62e91-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62e91-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="62e91-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62e91-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="62e91-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62e91-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62e91-149">This property is read-only.</span></span> <span data-ttu-id="62e91-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62e91-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62e91-151">createdDateTime</span></span>|<span data-ttu-id="62e91-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62e91-152">DateTimeOffset</span></span>|<span data-ttu-id="62e91-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="62e91-153">DateTime the object was created.</span></span> <span data-ttu-id="62e91-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62e91-155">description</span><span class="sxs-lookup"><span data-stu-id="62e91-155">description</span></span>|<span data-ttu-id="62e91-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62e91-156">String</span></span>|<span data-ttu-id="62e91-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="62e91-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62e91-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62e91-159">displayName</span><span class="sxs-lookup"><span data-stu-id="62e91-159">displayName</span></span>|<span data-ttu-id="62e91-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62e91-160">String</span></span>|<span data-ttu-id="62e91-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="62e91-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62e91-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62e91-163">Version</span><span class="sxs-lookup"><span data-stu-id="62e91-163">version</span></span>|<span data-ttu-id="62e91-164">Int32</span><span class="sxs-lookup"><span data-stu-id="62e91-164">Int32</span></span>|<span data-ttu-id="62e91-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="62e91-165">Version of the device configuration.</span></span> <span data-ttu-id="62e91-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62e91-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62e91-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="62e91-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="62e91-168">Int32</span><span class="sxs-lookup"><span data-stu-id="62e91-168">Int32</span></span>|<span data-ttu-id="62e91-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="62e91-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="62e91-170">Gültige Werte 1 bis 99 geerbt von [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62e91-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="62e91-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="62e91-171">subjectNameFormat</span></span>|[<span data-ttu-id="62e91-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="62e91-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="62e91-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="62e91-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="62e91-174">Von [AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="62e91-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="62e91-175">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="62e91-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="62e91-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="62e91-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="62e91-177">Int32</span><span class="sxs-lookup"><span data-stu-id="62e91-177">Int32</span></span>|<span data-ttu-id="62e91-178">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="62e91-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="62e91-179">Geerbt von [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62e91-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="62e91-180">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="62e91-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="62e91-181">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="62e91-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="62e91-182">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="62e91-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="62e91-183">Von [AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="62e91-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="62e91-184">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="62e91-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="62e91-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="62e91-185">extendedKeyUsages</span></span>|<span data-ttu-id="62e91-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="62e91-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="62e91-187">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="62e91-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="62e91-188">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="62e91-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="62e91-189">Geerbt von [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62e91-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="62e91-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="62e91-190">scepServerUrls</span></span>|<span data-ttu-id="62e91-191">String collection</span><span class="sxs-lookup"><span data-stu-id="62e91-191">String collection</span></span>|<span data-ttu-id="62e91-192">SCEP-Server-URL (s)</span><span class="sxs-lookup"><span data-stu-id="62e91-192">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="62e91-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="62e91-193">subjectNameFormatString</span></span>|<span data-ttu-id="62e91-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62e91-194">String</span></span>|<span data-ttu-id="62e91-195">Benutzerdefiniertes Format, das mit SubjectNameFormat = Custom verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="62e91-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="62e91-196">Beispiel: CN = {{Email Adresse}}, E = {Email Adresse}}, OU = Enterprise users, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="62e91-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="62e91-197">keyUsage</span><span class="sxs-lookup"><span data-stu-id="62e91-197">keyUsage</span></span>|[<span data-ttu-id="62e91-198">keyUsages</span><span class="sxs-lookup"><span data-stu-id="62e91-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="62e91-199">SCEP-Schlüsselverwendung.</span><span class="sxs-lookup"><span data-stu-id="62e91-199">SCEP Key Usage.</span></span> <span data-ttu-id="62e91-200">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="62e91-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="62e91-201">keySize</span><span class="sxs-lookup"><span data-stu-id="62e91-201">keySize</span></span>|[<span data-ttu-id="62e91-202">keySize</span><span class="sxs-lookup"><span data-stu-id="62e91-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="62e91-203">SCEP-Schlüsselgröße.</span><span class="sxs-lookup"><span data-stu-id="62e91-203">SCEP Key Size.</span></span> <span data-ttu-id="62e91-204">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="62e91-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="62e91-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="62e91-205">hashAlgorithm</span></span>|[<span data-ttu-id="62e91-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="62e91-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="62e91-207">SCEP-Hash Algorithmus.</span><span class="sxs-lookup"><span data-stu-id="62e91-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="62e91-208">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="62e91-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="62e91-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="62e91-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="62e91-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62e91-210">String</span></span>|<span data-ttu-id="62e91-211">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="62e91-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="62e91-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="62e91-212">certificateStore</span></span>|[<span data-ttu-id="62e91-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="62e91-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="62e91-214">Zielspeicher Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="62e91-214">Target store certificate.</span></span> <span data-ttu-id="62e91-215">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="62e91-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="62e91-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="62e91-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="62e91-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="62e91-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="62e91-218">Benutzerdefinierte Alterantive.</span><span class="sxs-lookup"><span data-stu-id="62e91-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="62e91-219">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="62e91-219">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="62e91-220">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="62e91-220">subjectAlternativeNameType</span></span>|[<span data-ttu-id="62e91-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="62e91-221">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="62e91-222">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="62e91-222">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="62e91-223">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="62e91-223">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="62e91-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="62e91-224">Response</span></span>
<span data-ttu-id="62e91-225">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="62e91-225">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62e91-226">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62e91-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="62e91-227">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62e91-227">Request</span></span>
<span data-ttu-id="62e91-228">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="62e91-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="62e91-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="62e91-229">Response</span></span>
<span data-ttu-id="62e91-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62e91-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```




