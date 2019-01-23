---
title: AndroidScepCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidScepCertificateProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b68cd2c1c5a4e55408e0aee6f7797ae08f52a88c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424112"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="3850f-103">AndroidScepCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3850f-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="3850f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3850f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3850f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3850f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3850f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3850f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3850f-107">Aktualisieren Sie die Eigenschaften eines [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3850f-107">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3850f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3850f-108">Prerequisites</span></span>
<span data-ttu-id="3850f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3850f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3850f-111">Permission type</span></span>|<span data-ttu-id="3850f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3850f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3850f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3850f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3850f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3850f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3850f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3850f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3850f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3850f-116">Not supported.</span></span>|
|<span data-ttu-id="3850f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3850f-117">Application</span></span>|<span data-ttu-id="3850f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3850f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3850f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3850f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3850f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3850f-120">Request headers</span></span>
|<span data-ttu-id="3850f-121">Header</span><span class="sxs-lookup"><span data-stu-id="3850f-121">Header</span></span>|<span data-ttu-id="3850f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3850f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3850f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3850f-123">Authorization</span></span>|<span data-ttu-id="3850f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3850f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3850f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3850f-125">Accept</span></span>|<span data-ttu-id="3850f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3850f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3850f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3850f-127">Request body</span></span>
<span data-ttu-id="3850f-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3850f-128">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="3850f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="3850f-129">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="3850f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3850f-130">Property</span></span>|<span data-ttu-id="3850f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3850f-131">Type</span></span>|<span data-ttu-id="3850f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3850f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3850f-133">id</span><span class="sxs-lookup"><span data-stu-id="3850f-133">id</span></span>|<span data-ttu-id="3850f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3850f-134">String</span></span>|<span data-ttu-id="3850f-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3850f-135">Key of the entity.</span></span> <span data-ttu-id="3850f-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3850f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3850f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3850f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3850f-138">DateTimeOffset</span></span>|<span data-ttu-id="3850f-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3850f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3850f-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3850f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3850f-141">roleScopeTagIds</span></span>|<span data-ttu-id="3850f-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3850f-142">String collection</span></span>|<span data-ttu-id="3850f-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="3850f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3850f-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3850f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3850f-145">supportsScopeTags</span></span>|<span data-ttu-id="3850f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3850f-146">Boolean</span></span>|<span data-ttu-id="3850f-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3850f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3850f-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="3850f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3850f-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="3850f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3850f-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3850f-150">This property is read-only.</span></span> <span data-ttu-id="3850f-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3850f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3850f-152">createdDateTime</span></span>|<span data-ttu-id="3850f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3850f-153">DateTimeOffset</span></span>|<span data-ttu-id="3850f-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3850f-154">DateTime the object was created.</span></span> <span data-ttu-id="3850f-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3850f-156">description</span><span class="sxs-lookup"><span data-stu-id="3850f-156">description</span></span>|<span data-ttu-id="3850f-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3850f-157">String</span></span>|<span data-ttu-id="3850f-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3850f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3850f-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3850f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3850f-160">displayName</span></span>|<span data-ttu-id="3850f-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3850f-161">String</span></span>|<span data-ttu-id="3850f-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3850f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3850f-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3850f-164">Version</span><span class="sxs-lookup"><span data-stu-id="3850f-164">version</span></span>|<span data-ttu-id="3850f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3850f-165">Int32</span></span>|<span data-ttu-id="3850f-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3850f-166">Version of the device configuration.</span></span> <span data-ttu-id="3850f-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3850f-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3850f-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="3850f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3850f-169">Int32</span></span>|<span data-ttu-id="3850f-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="3850f-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3850f-171">Gültige Werte 1 bis 99 Inherited aus [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3850f-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3850f-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3850f-172">subjectNameFormat</span></span>|[<span data-ttu-id="3850f-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3850f-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3850f-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="3850f-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="3850f-175">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3850f-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3850f-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3850f-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3850f-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3850f-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3850f-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3850f-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="3850f-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="3850f-180">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3850f-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3850f-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3850f-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3850f-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3850f-183">Int32</span><span class="sxs-lookup"><span data-stu-id="3850f-183">Int32</span></span>|<span data-ttu-id="3850f-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="3850f-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3850f-185">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3850f-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3850f-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3850f-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3850f-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3850f-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3850f-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="3850f-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3850f-189">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3850f-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3850f-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="3850f-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3850f-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="3850f-191">extendedKeyUsages</span></span>|<span data-ttu-id="3850f-192">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3850f-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="3850f-193">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="3850f-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="3850f-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="3850f-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3850f-195">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3850f-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3850f-196">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="3850f-196">scepServerUrls</span></span>|<span data-ttu-id="3850f-197">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3850f-197">String collection</span></span>|<span data-ttu-id="3850f-198">SCEP Server URL(s) hinzu</span><span class="sxs-lookup"><span data-stu-id="3850f-198">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="3850f-199">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3850f-199">subjectNameFormatString</span></span>|<span data-ttu-id="3850f-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3850f-200">String</span></span>|<span data-ttu-id="3850f-201">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="3850f-201">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="3850f-202">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="3850f-202">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="3850f-203">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="3850f-203">keyUsage</span></span>|[<span data-ttu-id="3850f-204">keyUsages</span><span class="sxs-lookup"><span data-stu-id="3850f-204">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="3850f-205">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="3850f-205">SCEP Key Usage.</span></span> <span data-ttu-id="3850f-206">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="3850f-206">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="3850f-207">keySize</span><span class="sxs-lookup"><span data-stu-id="3850f-207">keySize</span></span>|[<span data-ttu-id="3850f-208">keySize</span><span class="sxs-lookup"><span data-stu-id="3850f-208">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="3850f-209">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="3850f-209">SCEP Key Size.</span></span> <span data-ttu-id="3850f-210">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="3850f-210">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="3850f-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3850f-211">hashAlgorithm</span></span>|[<span data-ttu-id="3850f-212">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="3850f-212">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="3850f-213">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="3850f-213">SCEP Hash Algorithm.</span></span> <span data-ttu-id="3850f-214">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="3850f-214">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="3850f-215">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3850f-215">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3850f-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3850f-216">String</span></span>|<span data-ttu-id="3850f-217">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="3850f-217">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="3850f-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="3850f-218">Response</span></span>
<span data-ttu-id="3850f-219">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3850f-219">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3850f-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3850f-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="3850f-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3850f-221">Request</span></span>
<span data-ttu-id="3850f-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3850f-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="3850f-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="3850f-223">Response</span></span>
<span data-ttu-id="3850f-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3850f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




