---
title: AndroidImportedPFXCertificateProfile aktualisieren
description: Aktualisieren der Eigenschaften eines androidImportedPFXCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb3e207fd4abc0c51be11021da483823de05445d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173773"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="a5746-103">AndroidImportedPFXCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a5746-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="a5746-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5746-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5746-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a5746-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5746-106">Aktualisieren der Eigenschaften eines [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5746-106">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5746-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a5746-107">Prerequisites</span></span>
<span data-ttu-id="a5746-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a5746-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5746-110">Permission type</span></span>|<span data-ttu-id="a5746-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5746-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5746-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5746-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5746-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5746-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5746-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5746-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5746-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5746-115">Not supported.</span></span>|
|<span data-ttu-id="a5746-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5746-116">Application</span></span>|<span data-ttu-id="a5746-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5746-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5746-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5746-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a5746-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5746-119">Request headers</span></span>
|<span data-ttu-id="a5746-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a5746-120">Header</span></span>|<span data-ttu-id="a5746-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a5746-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5746-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5746-122">Authorization</span></span>|<span data-ttu-id="a5746-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a5746-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5746-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a5746-124">Accept</span></span>|<span data-ttu-id="a5746-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5746-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5746-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5746-126">Request body</span></span>
<span data-ttu-id="a5746-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a5746-127">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="a5746-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a5746-128">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="a5746-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5746-129">Property</span></span>|<span data-ttu-id="a5746-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a5746-130">Type</span></span>|<span data-ttu-id="a5746-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5746-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5746-132">id</span><span class="sxs-lookup"><span data-stu-id="a5746-132">id</span></span>|<span data-ttu-id="a5746-133">string</span><span class="sxs-lookup"><span data-stu-id="a5746-133">String</span></span>|<span data-ttu-id="a5746-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a5746-134">Key of the entity.</span></span> <span data-ttu-id="a5746-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5746-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5746-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a5746-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5746-137">DateTimeOffset</span></span>|<span data-ttu-id="a5746-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5746-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a5746-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5746-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="a5746-140">roleScopeTagIds</span></span>|<span data-ttu-id="a5746-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a5746-141">String collection</span></span>|<span data-ttu-id="a5746-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="a5746-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a5746-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5746-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a5746-144">supportsScopeTags</span></span>|<span data-ttu-id="a5746-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5746-145">Boolean</span></span>|<span data-ttu-id="a5746-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5746-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a5746-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="a5746-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a5746-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a5746-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a5746-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a5746-149">This property is read-only.</span></span> <span data-ttu-id="a5746-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5746-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5746-151">createdDateTime</span></span>|<span data-ttu-id="a5746-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5746-152">DateTimeOffset</span></span>|<span data-ttu-id="a5746-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5746-153">DateTime the object was created.</span></span> <span data-ttu-id="a5746-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5746-155">description</span><span class="sxs-lookup"><span data-stu-id="a5746-155">description</span></span>|<span data-ttu-id="a5746-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5746-156">String</span></span>|<span data-ttu-id="a5746-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a5746-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a5746-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5746-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a5746-159">displayName</span></span>|<span data-ttu-id="a5746-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5746-160">String</span></span>|<span data-ttu-id="a5746-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a5746-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a5746-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5746-163">Version</span><span class="sxs-lookup"><span data-stu-id="a5746-163">version</span></span>|<span data-ttu-id="a5746-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a5746-164">Int32</span></span>|<span data-ttu-id="a5746-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a5746-165">Version of the device configuration.</span></span> <span data-ttu-id="a5746-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5746-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5746-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="a5746-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="a5746-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a5746-168">Int32</span></span>|<span data-ttu-id="a5746-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="a5746-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a5746-170">Gültige Werte 1 bis 99 geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a5746-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a5746-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a5746-171">subjectNameFormat</span></span>|[<span data-ttu-id="a5746-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a5746-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a5746-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="a5746-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="a5746-174">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="a5746-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a5746-175">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a5746-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a5746-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a5746-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a5746-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a5746-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a5746-178">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="a5746-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a5746-179">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="a5746-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a5746-180">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a5746-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a5746-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a5746-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a5746-182">Int32</span><span class="sxs-lookup"><span data-stu-id="a5746-182">Int32</span></span>|<span data-ttu-id="a5746-183">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a5746-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a5746-184">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a5746-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a5746-185">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="a5746-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a5746-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="a5746-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a5746-187">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a5746-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a5746-188">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="a5746-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a5746-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="a5746-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a5746-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a5746-190">extendedKeyUsages</span></span>|<span data-ttu-id="a5746-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="a5746-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a5746-192">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="a5746-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a5746-193">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a5746-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a5746-194">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a5746-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a5746-195">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a5746-195">intendedPurpose</span></span>|[<span data-ttu-id="a5746-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a5746-196">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="a5746-197">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a5746-197">Not yet documented.</span></span> <span data-ttu-id="a5746-198">Mögliche Werte: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="a5746-198">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="a5746-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5746-199">Response</span></span>
<span data-ttu-id="a5746-200">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a5746-200">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5746-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5746-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5746-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5746-202">Request</span></span>
<span data-ttu-id="a5746-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5746-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 719

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="a5746-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5746-204">Response</span></span>
<span data-ttu-id="a5746-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5746-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 891

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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
  "intendedPurpose": "smimeEncryption"
}
```




