---
title: AndroidForWorkImportedPFXCertificateProfile aktualisieren
description: Aktualisieren der Eigenschaften eines androidForWorkImportedPFXCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8787e52639878ae2ea799678d2174162fd369f43
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960748"
---
# <a name="update-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="e5738-103">AndroidForWorkImportedPFXCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e5738-103">Update androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="e5738-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5738-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5738-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e5738-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5738-106">Aktualisieren der Eigenschaften eines [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e5738-106">Update the properties of a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5738-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e5738-107">Prerequisites</span></span>
<span data-ttu-id="e5738-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5738-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5738-110">Permission type</span></span>|<span data-ttu-id="e5738-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5738-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5738-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5738-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5738-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5738-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5738-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5738-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5738-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5738-115">Not supported.</span></span>|
|<span data-ttu-id="e5738-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5738-116">Application</span></span>|<span data-ttu-id="e5738-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5738-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5738-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5738-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e5738-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e5738-119">Request headers</span></span>
|<span data-ttu-id="e5738-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e5738-120">Header</span></span>|<span data-ttu-id="e5738-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e5738-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5738-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5738-122">Authorization</span></span>|<span data-ttu-id="e5738-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e5738-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5738-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e5738-124">Accept</span></span>|<span data-ttu-id="e5738-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5738-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5738-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e5738-126">Request body</span></span>
<span data-ttu-id="e5738-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="e5738-127">In the request body, supply a JSON representation for the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="e5738-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e5738-128">The following table shows the properties that are required when you create the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="e5738-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e5738-129">Property</span></span>|<span data-ttu-id="e5738-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e5738-130">Type</span></span>|<span data-ttu-id="e5738-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5738-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5738-132">id</span><span class="sxs-lookup"><span data-stu-id="e5738-132">id</span></span>|<span data-ttu-id="e5738-133">String</span><span class="sxs-lookup"><span data-stu-id="e5738-133">String</span></span>|<span data-ttu-id="e5738-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e5738-134">Key of the entity.</span></span> <span data-ttu-id="e5738-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5738-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5738-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5738-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e5738-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5738-137">DateTimeOffset</span></span>|<span data-ttu-id="e5738-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e5738-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e5738-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5738-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5738-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="e5738-140">roleScopeTagIds</span></span>|<span data-ttu-id="e5738-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e5738-141">String collection</span></span>|<span data-ttu-id="e5738-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="e5738-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5738-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5738-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5738-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e5738-144">supportsScopeTags</span></span>|<span data-ttu-id="e5738-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e5738-145">Boolean</span></span>|<span data-ttu-id="e5738-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5738-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e5738-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="e5738-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e5738-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="e5738-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e5738-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e5738-149">This property is read-only.</span></span> <span data-ttu-id="e5738-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5738-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5738-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5738-151">createdDateTime</span></span>|<span data-ttu-id="e5738-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5738-152">DateTimeOffset</span></span>|<span data-ttu-id="e5738-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e5738-153">DateTime the object was created.</span></span> <span data-ttu-id="e5738-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5738-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5738-155">description</span><span class="sxs-lookup"><span data-stu-id="e5738-155">description</span></span>|<span data-ttu-id="e5738-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e5738-156">String</span></span>|<span data-ttu-id="e5738-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e5738-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5738-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5738-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5738-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e5738-159">displayName</span></span>|<span data-ttu-id="e5738-160">String</span><span class="sxs-lookup"><span data-stu-id="e5738-160">String</span></span>|<span data-ttu-id="e5738-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e5738-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5738-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5738-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5738-163">Version</span><span class="sxs-lookup"><span data-stu-id="e5738-163">version</span></span>|<span data-ttu-id="e5738-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e5738-164">Int32</span></span>|<span data-ttu-id="e5738-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e5738-165">Version of the device configuration.</span></span> <span data-ttu-id="e5738-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5738-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5738-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="e5738-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="e5738-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e5738-168">Int32</span></span>|<span data-ttu-id="e5738-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="e5738-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e5738-170">Gültige Werte 1 bis 99 geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e5738-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e5738-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e5738-171">subjectNameFormat</span></span>|[<span data-ttu-id="e5738-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e5738-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="e5738-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="e5738-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="e5738-174">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e5738-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="e5738-175">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="e5738-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="e5738-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e5738-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="e5738-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e5738-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e5738-178">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="e5738-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="e5738-179">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e5738-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="e5738-180">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="e5738-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e5738-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e5738-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e5738-182">Int32</span><span class="sxs-lookup"><span data-stu-id="e5738-182">Int32</span></span>|<span data-ttu-id="e5738-183">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="e5738-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="e5738-184">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e5738-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e5738-185">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="e5738-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e5738-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="e5738-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e5738-187">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="e5738-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e5738-188">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e5738-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="e5738-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="e5738-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e5738-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="e5738-190">extendedKeyUsages</span></span>|<span data-ttu-id="e5738-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="e5738-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="e5738-192">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="e5738-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="e5738-193">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e5738-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e5738-194">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e5738-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e5738-195">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="e5738-195">intendedPurpose</span></span>|[<span data-ttu-id="e5738-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="e5738-196">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="e5738-197">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e5738-197">Not yet documented.</span></span> <span data-ttu-id="e5738-198">Mögliche Werte: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="e5738-198">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="e5738-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5738-199">Response</span></span>
<span data-ttu-id="e5738-200">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e5738-200">If successful, this method returns a `200 OK` response code and an updated [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5738-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5738-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5738-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5738-202">Request</span></span>
<span data-ttu-id="e5738-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e5738-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="e5738-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5738-204">Response</span></span>
<span data-ttu-id="e5738-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5738-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




