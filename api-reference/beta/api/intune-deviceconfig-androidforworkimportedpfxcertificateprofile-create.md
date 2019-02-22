---
title: AndroidForWorkImportedPFXCertificateProfile erstellen
description: Erstellen eines neuen androidForWorkImportedPFXCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b4c2ffde1683ab2a7100604405d4b35a85d6931
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166899"
---
# <a name="create-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="15e65-103">AndroidForWorkImportedPFXCertificateProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="15e65-103">Create androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="15e65-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15e65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15e65-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="15e65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15e65-106">Erstellen eines neuen [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="15e65-106">Create a new [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15e65-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15e65-107">Prerequisites</span></span>
<span data-ttu-id="15e65-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15e65-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15e65-110">Permission type</span></span>|<span data-ttu-id="15e65-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15e65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15e65-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15e65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15e65-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15e65-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15e65-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15e65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15e65-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15e65-115">Not supported.</span></span>|
|<span data-ttu-id="15e65-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15e65-116">Application</span></span>|<span data-ttu-id="15e65-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15e65-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15e65-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15e65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15e65-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15e65-119">Request headers</span></span>
|<span data-ttu-id="15e65-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="15e65-120">Header</span></span>|<span data-ttu-id="15e65-121">Wert</span><span class="sxs-lookup"><span data-stu-id="15e65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15e65-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15e65-122">Authorization</span></span>|<span data-ttu-id="15e65-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15e65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15e65-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="15e65-124">Accept</span></span>|<span data-ttu-id="15e65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15e65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15e65-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15e65-126">Request body</span></span>
<span data-ttu-id="15e65-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidForWorkImportedPFXCertificateProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="15e65-127">In the request body, supply a JSON representation for the androidForWorkImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="15e65-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidForWorkImportedPFXCertificateProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="15e65-128">The following table shows the properties that are required when you create the androidForWorkImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="15e65-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15e65-129">Property</span></span>|<span data-ttu-id="15e65-130">Typ</span><span class="sxs-lookup"><span data-stu-id="15e65-130">Type</span></span>|<span data-ttu-id="15e65-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15e65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15e65-132">id</span><span class="sxs-lookup"><span data-stu-id="15e65-132">id</span></span>|<span data-ttu-id="15e65-133">string</span><span class="sxs-lookup"><span data-stu-id="15e65-133">String</span></span>|<span data-ttu-id="15e65-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="15e65-134">Key of the entity.</span></span> <span data-ttu-id="15e65-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15e65-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15e65-136">lastModifiedDateTime</span></span>|<span data-ttu-id="15e65-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15e65-137">DateTimeOffset</span></span>|<span data-ttu-id="15e65-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="15e65-138">DateTime the object was last modified.</span></span> <span data-ttu-id="15e65-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15e65-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="15e65-140">roleScopeTagIds</span></span>|<span data-ttu-id="15e65-141">String collection</span><span class="sxs-lookup"><span data-stu-id="15e65-141">String collection</span></span>|<span data-ttu-id="15e65-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="15e65-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15e65-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15e65-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="15e65-144">supportsScopeTags</span></span>|<span data-ttu-id="15e65-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="15e65-145">Boolean</span></span>|<span data-ttu-id="15e65-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15e65-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="15e65-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="15e65-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="15e65-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="15e65-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="15e65-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="15e65-149">This property is read-only.</span></span> <span data-ttu-id="15e65-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15e65-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15e65-151">createdDateTime</span></span>|<span data-ttu-id="15e65-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15e65-152">DateTimeOffset</span></span>|<span data-ttu-id="15e65-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="15e65-153">DateTime the object was created.</span></span> <span data-ttu-id="15e65-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15e65-155">description</span><span class="sxs-lookup"><span data-stu-id="15e65-155">description</span></span>|<span data-ttu-id="15e65-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15e65-156">String</span></span>|<span data-ttu-id="15e65-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="15e65-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15e65-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15e65-159">displayName</span><span class="sxs-lookup"><span data-stu-id="15e65-159">displayName</span></span>|<span data-ttu-id="15e65-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15e65-160">String</span></span>|<span data-ttu-id="15e65-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="15e65-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15e65-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15e65-163">Version</span><span class="sxs-lookup"><span data-stu-id="15e65-163">version</span></span>|<span data-ttu-id="15e65-164">Int32</span><span class="sxs-lookup"><span data-stu-id="15e65-164">Int32</span></span>|<span data-ttu-id="15e65-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="15e65-165">Version of the device configuration.</span></span> <span data-ttu-id="15e65-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15e65-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15e65-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="15e65-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="15e65-168">Int32</span><span class="sxs-lookup"><span data-stu-id="15e65-168">Int32</span></span>|<span data-ttu-id="15e65-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="15e65-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="15e65-170">Gültige Werte 1 bis 99 geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="15e65-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="15e65-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="15e65-171">subjectNameFormat</span></span>|[<span data-ttu-id="15e65-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="15e65-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="15e65-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="15e65-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="15e65-174">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="15e65-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="15e65-175">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="15e65-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="15e65-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="15e65-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="15e65-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="15e65-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="15e65-178">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="15e65-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="15e65-179">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="15e65-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="15e65-180">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="15e65-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="15e65-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="15e65-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="15e65-182">Int32</span><span class="sxs-lookup"><span data-stu-id="15e65-182">Int32</span></span>|<span data-ttu-id="15e65-183">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="15e65-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="15e65-184">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="15e65-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="15e65-185">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="15e65-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="15e65-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="15e65-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="15e65-187">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="15e65-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="15e65-188">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="15e65-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="15e65-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="15e65-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="15e65-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="15e65-190">extendedKeyUsages</span></span>|<span data-ttu-id="15e65-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="15e65-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="15e65-192">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="15e65-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="15e65-193">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="15e65-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="15e65-194">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="15e65-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="15e65-195">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="15e65-195">intendedPurpose</span></span>|[<span data-ttu-id="15e65-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="15e65-196">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="15e65-197">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="15e65-197">Not yet documented.</span></span> <span data-ttu-id="15e65-198">Mögliche Werte: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="15e65-198">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="15e65-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="15e65-199">Response</span></span>
<span data-ttu-id="15e65-200">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="15e65-200">If successful, this method returns a `201 Created` response code and a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15e65-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15e65-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="15e65-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15e65-202">Request</span></span>
<span data-ttu-id="15e65-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15e65-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 726

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="15e65-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="15e65-204">Response</span></span>
<span data-ttu-id="15e65-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15e65-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 898

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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




