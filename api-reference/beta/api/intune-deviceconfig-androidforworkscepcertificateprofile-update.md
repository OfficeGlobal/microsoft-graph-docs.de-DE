---
title: AndroidForWorkScepCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkScepCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e034b7c4dde6a6dbbfc1de41a2d5ea25c7d8f49f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946721"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="5020e-103">AndroidForWorkScepCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5020e-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="5020e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5020e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5020e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5020e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5020e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5020e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5020e-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5020e-107">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5020e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5020e-108">Prerequisites</span></span>
<span data-ttu-id="5020e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5020e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5020e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5020e-111">Permission type</span></span>|<span data-ttu-id="5020e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5020e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5020e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5020e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5020e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5020e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5020e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5020e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5020e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5020e-116">Not supported.</span></span>|
|<span data-ttu-id="5020e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5020e-117">Application</span></span>|<span data-ttu-id="5020e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5020e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5020e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5020e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5020e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5020e-120">Request headers</span></span>
|<span data-ttu-id="5020e-121">Header</span><span class="sxs-lookup"><span data-stu-id="5020e-121">Header</span></span>|<span data-ttu-id="5020e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5020e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5020e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5020e-123">Authorization</span></span>|<span data-ttu-id="5020e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5020e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5020e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5020e-125">Accept</span></span>|<span data-ttu-id="5020e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5020e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5020e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5020e-127">Request body</span></span>
<span data-ttu-id="5020e-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5020e-128">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="5020e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5020e-129">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="5020e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5020e-130">Property</span></span>|<span data-ttu-id="5020e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5020e-131">Type</span></span>|<span data-ttu-id="5020e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5020e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5020e-133">id</span><span class="sxs-lookup"><span data-stu-id="5020e-133">id</span></span>|<span data-ttu-id="5020e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5020e-134">String</span></span>|<span data-ttu-id="5020e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5020e-135">Key of the entity.</span></span> <span data-ttu-id="5020e-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5020e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5020e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5020e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5020e-138">DateTimeOffset</span></span>|<span data-ttu-id="5020e-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5020e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5020e-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5020e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5020e-141">roleScopeTagIds</span></span>|<span data-ttu-id="5020e-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="5020e-142">String collection</span></span>|<span data-ttu-id="5020e-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="5020e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5020e-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5020e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5020e-145">supportsScopeTags</span></span>|<span data-ttu-id="5020e-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5020e-146">Boolean</span></span>|<span data-ttu-id="5020e-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5020e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5020e-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="5020e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5020e-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="5020e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5020e-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5020e-150">This property is read-only.</span></span> <span data-ttu-id="5020e-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5020e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5020e-152">createdDateTime</span></span>|<span data-ttu-id="5020e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5020e-153">DateTimeOffset</span></span>|<span data-ttu-id="5020e-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5020e-154">DateTime the object was created.</span></span> <span data-ttu-id="5020e-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5020e-156">description</span><span class="sxs-lookup"><span data-stu-id="5020e-156">description</span></span>|<span data-ttu-id="5020e-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5020e-157">String</span></span>|<span data-ttu-id="5020e-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5020e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5020e-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5020e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5020e-160">displayName</span></span>|<span data-ttu-id="5020e-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5020e-161">String</span></span>|<span data-ttu-id="5020e-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5020e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5020e-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5020e-164">Version</span><span class="sxs-lookup"><span data-stu-id="5020e-164">version</span></span>|<span data-ttu-id="5020e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5020e-165">Int32</span></span>|<span data-ttu-id="5020e-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5020e-166">Version of the device configuration.</span></span> <span data-ttu-id="5020e-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5020e-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5020e-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="5020e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="5020e-169">Int32</span></span>|<span data-ttu-id="5020e-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="5020e-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5020e-171">Gültige Werte 1 bis 99 Inherited aus [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5020e-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5020e-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5020e-172">subjectNameFormat</span></span>|[<span data-ttu-id="5020e-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5020e-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="5020e-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="5020e-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="5020e-175">Geerbt von [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="5020e-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="5020e-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="5020e-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5020e-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5020e-178">Int32</span><span class="sxs-lookup"><span data-stu-id="5020e-178">Int32</span></span>|<span data-ttu-id="5020e-179">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="5020e-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5020e-180">Geerbt von [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5020e-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5020e-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5020e-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5020e-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5020e-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5020e-183">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="5020e-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5020e-184">Geerbt von [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5020e-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="5020e-185">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="5020e-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5020e-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="5020e-186">extendedKeyUsages</span></span>|<span data-ttu-id="5020e-187">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5020e-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="5020e-188">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="5020e-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="5020e-189">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5020e-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5020e-190">Geerbt von [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5020e-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5020e-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="5020e-191">scepServerUrls</span></span>|<span data-ttu-id="5020e-192">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="5020e-192">String collection</span></span>|<span data-ttu-id="5020e-193">SCEP Server URL(s) hinzu</span><span class="sxs-lookup"><span data-stu-id="5020e-193">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="5020e-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5020e-194">subjectNameFormatString</span></span>|<span data-ttu-id="5020e-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5020e-195">String</span></span>|<span data-ttu-id="5020e-196">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="5020e-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="5020e-197">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="5020e-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="5020e-198">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="5020e-198">keyUsage</span></span>|[<span data-ttu-id="5020e-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="5020e-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="5020e-200">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="5020e-200">SCEP Key Usage.</span></span> <span data-ttu-id="5020e-201">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="5020e-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="5020e-202">keySize</span><span class="sxs-lookup"><span data-stu-id="5020e-202">keySize</span></span>|[<span data-ttu-id="5020e-203">keySize</span><span class="sxs-lookup"><span data-stu-id="5020e-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="5020e-204">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="5020e-204">SCEP Key Size.</span></span> <span data-ttu-id="5020e-205">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="5020e-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="5020e-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="5020e-206">hashAlgorithm</span></span>|[<span data-ttu-id="5020e-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="5020e-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="5020e-208">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="5020e-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="5020e-209">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="5020e-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="5020e-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5020e-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5020e-211">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5020e-211">String</span></span>|<span data-ttu-id="5020e-212">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="5020e-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="5020e-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5020e-213">certificateStore</span></span>|[<span data-ttu-id="5020e-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5020e-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="5020e-215">Ziel-Zertifikatspeicher.</span><span class="sxs-lookup"><span data-stu-id="5020e-215">Target store certificate.</span></span> <span data-ttu-id="5020e-216">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="5020e-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="5020e-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="5020e-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="5020e-218">[CustomSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5020e-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="5020e-219">Benutzerdefinierte Subject Name Alterantive Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="5020e-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="5020e-220">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5020e-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5020e-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5020e-221">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5020e-222">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5020e-222">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5020e-223">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="5020e-223">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="5020e-224">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5020e-224">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="5020e-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="5020e-225">Response</span></span>
<span data-ttu-id="5020e-226">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5020e-226">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5020e-227">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5020e-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="5020e-228">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5020e-228">Request</span></span>
<span data-ttu-id="5020e-229">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5020e-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1194

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

### <a name="response"></a><span data-ttu-id="5020e-230">Antwort</span><span class="sxs-lookup"><span data-stu-id="5020e-230">Response</span></span>
<span data-ttu-id="5020e-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5020e-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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





