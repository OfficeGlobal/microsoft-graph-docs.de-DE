---
title: AndroidImportedPFXCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidImportedPFXCertificateProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4eee0ad39bd7b39240961bd193118d7eed5d963b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397176"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="96784-103">AndroidImportedPFXCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="96784-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="96784-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="96784-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="96784-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96784-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96784-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96784-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96784-107">Aktualisieren Sie die Eigenschaften eines [AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="96784-107">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96784-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="96784-108">Prerequisites</span></span>
<span data-ttu-id="96784-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="96784-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="96784-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96784-111">Permission type</span></span>|<span data-ttu-id="96784-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96784-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96784-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96784-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96784-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96784-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96784-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96784-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96784-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96784-116">Not supported.</span></span>|
|<span data-ttu-id="96784-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96784-117">Application</span></span>|<span data-ttu-id="96784-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96784-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96784-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96784-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="96784-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96784-120">Request headers</span></span>
|<span data-ttu-id="96784-121">Header</span><span class="sxs-lookup"><span data-stu-id="96784-121">Header</span></span>|<span data-ttu-id="96784-122">Wert</span><span class="sxs-lookup"><span data-stu-id="96784-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96784-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="96784-123">Authorization</span></span>|<span data-ttu-id="96784-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="96784-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96784-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="96784-125">Accept</span></span>|<span data-ttu-id="96784-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96784-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96784-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96784-127">Request body</span></span>
<span data-ttu-id="96784-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="96784-128">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="96784-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="96784-129">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="96784-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96784-130">Property</span></span>|<span data-ttu-id="96784-131">Typ</span><span class="sxs-lookup"><span data-stu-id="96784-131">Type</span></span>|<span data-ttu-id="96784-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96784-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96784-133">id</span><span class="sxs-lookup"><span data-stu-id="96784-133">id</span></span>|<span data-ttu-id="96784-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96784-134">String</span></span>|<span data-ttu-id="96784-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="96784-135">Key of the entity.</span></span> <span data-ttu-id="96784-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96784-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96784-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96784-137">lastModifiedDateTime</span></span>|<span data-ttu-id="96784-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96784-138">DateTimeOffset</span></span>|<span data-ttu-id="96784-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="96784-139">DateTime the object was last modified.</span></span> <span data-ttu-id="96784-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96784-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96784-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96784-141">roleScopeTagIds</span></span>|<span data-ttu-id="96784-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="96784-142">String collection</span></span>|<span data-ttu-id="96784-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="96784-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="96784-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96784-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96784-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="96784-145">supportsScopeTags</span></span>|<span data-ttu-id="96784-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="96784-146">Boolean</span></span>|<span data-ttu-id="96784-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96784-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="96784-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="96784-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="96784-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="96784-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="96784-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="96784-150">This property is read-only.</span></span> <span data-ttu-id="96784-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96784-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96784-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96784-152">createdDateTime</span></span>|<span data-ttu-id="96784-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96784-153">DateTimeOffset</span></span>|<span data-ttu-id="96784-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="96784-154">DateTime the object was created.</span></span> <span data-ttu-id="96784-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96784-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96784-156">description</span><span class="sxs-lookup"><span data-stu-id="96784-156">description</span></span>|<span data-ttu-id="96784-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96784-157">String</span></span>|<span data-ttu-id="96784-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="96784-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96784-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96784-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96784-160">displayName</span><span class="sxs-lookup"><span data-stu-id="96784-160">displayName</span></span>|<span data-ttu-id="96784-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96784-161">String</span></span>|<span data-ttu-id="96784-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="96784-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96784-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96784-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96784-164">Version</span><span class="sxs-lookup"><span data-stu-id="96784-164">version</span></span>|<span data-ttu-id="96784-165">Int32</span><span class="sxs-lookup"><span data-stu-id="96784-165">Int32</span></span>|<span data-ttu-id="96784-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="96784-166">Version of the device configuration.</span></span> <span data-ttu-id="96784-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96784-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96784-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="96784-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="96784-169">Int32</span><span class="sxs-lookup"><span data-stu-id="96784-169">Int32</span></span>|<span data-ttu-id="96784-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="96784-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="96784-171">Gültige Werte 1 bis 99 Inherited aus [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96784-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="96784-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="96784-172">subjectNameFormat</span></span>|[<span data-ttu-id="96784-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="96784-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="96784-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="96784-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="96784-175">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="96784-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="96784-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="96784-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="96784-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="96784-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="96784-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="96784-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="96784-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="96784-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="96784-180">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="96784-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="96784-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="96784-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="96784-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="96784-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="96784-183">Int32</span><span class="sxs-lookup"><span data-stu-id="96784-183">Int32</span></span>|<span data-ttu-id="96784-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="96784-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="96784-185">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96784-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="96784-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="96784-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="96784-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="96784-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="96784-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="96784-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="96784-189">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="96784-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="96784-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="96784-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="96784-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="96784-191">extendedKeyUsages</span></span>|<span data-ttu-id="96784-192">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="96784-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="96784-193">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="96784-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="96784-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="96784-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="96784-195">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96784-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="96784-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="96784-196">intendedPurpose</span></span>|[<span data-ttu-id="96784-197">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="96784-197">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="96784-198">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="96784-198">Not yet documented.</span></span> <span data-ttu-id="96784-199">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="96784-199">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="96784-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="96784-200">Response</span></span>
<span data-ttu-id="96784-201">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="96784-201">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96784-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96784-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="96784-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96784-203">Request</span></span>
<span data-ttu-id="96784-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96784-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96784-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="96784-205">Response</span></span>
<span data-ttu-id="96784-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96784-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




