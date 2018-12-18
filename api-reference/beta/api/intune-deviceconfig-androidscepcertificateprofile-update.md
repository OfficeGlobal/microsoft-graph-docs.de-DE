---
title: AndroidScepCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidScepCertificateProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: 0728abf6983593de11afb6d0a08b8451b8fa5474
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348153"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="a6c3d-103">AndroidScepCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a6c3d-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="a6c3d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6c3d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6c3d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6c3d-107">Aktualisieren Sie die Eigenschaften eines [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-107">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6c3d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a6c3d-108">Prerequisites</span></span>
<span data-ttu-id="a6c3d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c3d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6c3d-111">Permission type</span></span>|<span data-ttu-id="a6c3d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6c3d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6c3d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6c3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6c3d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c3d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6c3d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6c3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c3d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6c3d-116">Not supported.</span></span>|
|<span data-ttu-id="a6c3d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6c3d-117">Application</span></span>|<span data-ttu-id="a6c3d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6c3d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6c3d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6c3d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6c3d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6c3d-120">Request headers</span></span>
|<span data-ttu-id="a6c3d-121">Header</span><span class="sxs-lookup"><span data-stu-id="a6c3d-121">Header</span></span>|<span data-ttu-id="a6c3d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a6c3d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6c3d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a6c3d-123">Authorization</span></span>|<span data-ttu-id="a6c3d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a6c3d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6c3d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6c3d-125">Accept</span></span>|<span data-ttu-id="a6c3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6c3d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c3d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6c3d-127">Request body</span></span>
<span data-ttu-id="a6c3d-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-128">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="a6c3d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-129">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="a6c3d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6c3d-130">Property</span></span>|<span data-ttu-id="a6c3d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a6c3d-131">Type</span></span>|<span data-ttu-id="a6c3d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6c3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c3d-133">id</span><span class="sxs-lookup"><span data-stu-id="a6c3d-133">id</span></span>|<span data-ttu-id="a6c3d-134">String</span><span class="sxs-lookup"><span data-stu-id="a6c3d-134">String</span></span>|<span data-ttu-id="a6c3d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a6c3d-135">Key of the entity.</span></span> <span data-ttu-id="a6c3d-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c3d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c3d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a6c3d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c3d-138">DateTimeOffset</span></span>|<span data-ttu-id="a6c3d-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a6c3d-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c3d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6c3d-141">roleScopeTagIds</span></span>|<span data-ttu-id="a6c3d-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a6c3d-142">String collection</span></span>|<span data-ttu-id="a6c3d-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a6c3d-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c3d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a6c3d-145">supportsScopeTags</span></span>|<span data-ttu-id="a6c3d-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a6c3d-146">Boolean</span></span>|<span data-ttu-id="a6c3d-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a6c3d-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a6c3d-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a6c3d-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-150">This property is read-only.</span></span> <span data-ttu-id="a6c3d-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c3d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c3d-152">createdDateTime</span></span>|<span data-ttu-id="a6c3d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c3d-153">DateTimeOffset</span></span>|<span data-ttu-id="a6c3d-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-154">DateTime the object was created.</span></span> <span data-ttu-id="a6c3d-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c3d-156">description</span><span class="sxs-lookup"><span data-stu-id="a6c3d-156">description</span></span>|<span data-ttu-id="a6c3d-157">String</span><span class="sxs-lookup"><span data-stu-id="a6c3d-157">String</span></span>|<span data-ttu-id="a6c3d-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6c3d-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c3d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a6c3d-160">displayName</span></span>|<span data-ttu-id="a6c3d-161">String</span><span class="sxs-lookup"><span data-stu-id="a6c3d-161">String</span></span>|<span data-ttu-id="a6c3d-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6c3d-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c3d-164">Version</span><span class="sxs-lookup"><span data-stu-id="a6c3d-164">version</span></span>|<span data-ttu-id="a6c3d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a6c3d-165">Int32</span></span>|<span data-ttu-id="a6c3d-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-166">Version of the device configuration.</span></span> <span data-ttu-id="a6c3d-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c3d-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a6c3d-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="a6c3d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a6c3d-169">Int32</span></span>|<span data-ttu-id="a6c3d-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a6c3d-171">Gültige Werte 1 bis 99 Inherited aus [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a6c3d-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a6c3d-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a6c3d-172">subjectNameFormat</span></span>|[<span data-ttu-id="a6c3d-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a6c3d-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a6c3d-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="a6c3d-175">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a6c3d-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a6c3d-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a6c3d-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a6c3d-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a6c3d-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a6c3d-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a6c3d-180">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a6c3d-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a6c3d-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a6c3d-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a6c3d-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a6c3d-183">Int32</span></span>|<span data-ttu-id="a6c3d-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a6c3d-185">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a6c3d-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a6c3d-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a6c3d-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a6c3d-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a6c3d-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a6c3d-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a6c3d-189">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a6c3d-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a6c3d-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a6c3d-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a6c3d-191">extendedKeyUsages</span></span>|<span data-ttu-id="a6c3d-192">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a6c3d-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a6c3d-193">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a6c3d-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a6c3d-195">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a6c3d-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a6c3d-196">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="a6c3d-196">scepServerUrls</span></span>|<span data-ttu-id="a6c3d-197">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a6c3d-197">String collection</span></span>|<span data-ttu-id="a6c3d-198">SCEP Server URL(s) hinzu</span><span class="sxs-lookup"><span data-stu-id="a6c3d-198">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="a6c3d-199">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a6c3d-199">subjectNameFormatString</span></span>|<span data-ttu-id="a6c3d-200">String</span><span class="sxs-lookup"><span data-stu-id="a6c3d-200">String</span></span>|<span data-ttu-id="a6c3d-201">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-201">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a6c3d-202">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="a6c3d-202">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a6c3d-203">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="a6c3d-203">keyUsage</span></span>|[<span data-ttu-id="a6c3d-204">keyUsages</span><span class="sxs-lookup"><span data-stu-id="a6c3d-204">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a6c3d-205">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-205">SCEP Key Usage.</span></span> <span data-ttu-id="a6c3d-206">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-206">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a6c3d-207">keySize</span><span class="sxs-lookup"><span data-stu-id="a6c3d-207">keySize</span></span>|[<span data-ttu-id="a6c3d-208">keySize</span><span class="sxs-lookup"><span data-stu-id="a6c3d-208">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="a6c3d-209">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-209">SCEP Key Size.</span></span> <span data-ttu-id="a6c3d-210">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-210">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="a6c3d-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a6c3d-211">hashAlgorithm</span></span>|[<span data-ttu-id="a6c3d-212">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="a6c3d-212">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="a6c3d-213">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-213">SCEP Hash Algorithm.</span></span> <span data-ttu-id="a6c3d-214">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-214">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="a6c3d-215">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a6c3d-215">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a6c3d-216">String</span><span class="sxs-lookup"><span data-stu-id="a6c3d-216">String</span></span>|<span data-ttu-id="a6c3d-217">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-217">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="a6c3d-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6c3d-218">Response</span></span>
<span data-ttu-id="a6c3d-219">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-219">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c3d-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6c3d-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6c3d-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6c3d-221">Request</span></span>
<span data-ttu-id="a6c3d-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 970

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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="a6c3d-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6c3d-223">Response</span></span>
<span data-ttu-id="a6c3d-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6c3d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1146

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





