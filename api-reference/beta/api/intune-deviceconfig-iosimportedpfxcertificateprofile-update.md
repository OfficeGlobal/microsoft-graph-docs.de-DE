---
title: IosImportedPFXCertificateProfile aktualisieren
description: Aktualisieren der Eigenschaften eines iosImportedPFXCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 744e30f9f869515184c915cba51232fb8a90b121
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161194"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="20737-103">IosImportedPFXCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="20737-103">Update iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="20737-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20737-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20737-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="20737-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20737-106">Aktualisieren der Eigenschaften eines [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="20737-106">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20737-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="20737-107">Prerequisites</span></span>
<span data-ttu-id="20737-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="20737-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="20737-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20737-110">Permission type</span></span>|<span data-ttu-id="20737-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20737-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20737-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20737-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20737-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20737-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20737-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20737-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20737-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20737-115">Not supported.</span></span>|
|<span data-ttu-id="20737-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20737-116">Application</span></span>|<span data-ttu-id="20737-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20737-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20737-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20737-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="20737-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20737-119">Request headers</span></span>
|<span data-ttu-id="20737-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="20737-120">Header</span></span>|<span data-ttu-id="20737-121">Wert</span><span class="sxs-lookup"><span data-stu-id="20737-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20737-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20737-122">Authorization</span></span>|<span data-ttu-id="20737-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="20737-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20737-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="20737-124">Accept</span></span>|<span data-ttu-id="20737-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20737-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20737-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20737-126">Request body</span></span>
<span data-ttu-id="20737-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="20737-127">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="20737-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="20737-128">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="20737-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20737-129">Property</span></span>|<span data-ttu-id="20737-130">Typ</span><span class="sxs-lookup"><span data-stu-id="20737-130">Type</span></span>|<span data-ttu-id="20737-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20737-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20737-132">id</span><span class="sxs-lookup"><span data-stu-id="20737-132">id</span></span>|<span data-ttu-id="20737-133">string</span><span class="sxs-lookup"><span data-stu-id="20737-133">String</span></span>|<span data-ttu-id="20737-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="20737-134">Key of the entity.</span></span> <span data-ttu-id="20737-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20737-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20737-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20737-136">lastModifiedDateTime</span></span>|<span data-ttu-id="20737-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20737-137">DateTimeOffset</span></span>|<span data-ttu-id="20737-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="20737-138">DateTime the object was last modified.</span></span> <span data-ttu-id="20737-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20737-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20737-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="20737-140">roleScopeTagIds</span></span>|<span data-ttu-id="20737-141">String collection</span><span class="sxs-lookup"><span data-stu-id="20737-141">String collection</span></span>|<span data-ttu-id="20737-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="20737-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="20737-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20737-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20737-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="20737-144">supportsScopeTags</span></span>|<span data-ttu-id="20737-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="20737-145">Boolean</span></span>|<span data-ttu-id="20737-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20737-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="20737-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="20737-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="20737-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="20737-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="20737-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="20737-149">This property is read-only.</span></span> <span data-ttu-id="20737-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20737-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20737-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20737-151">createdDateTime</span></span>|<span data-ttu-id="20737-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20737-152">DateTimeOffset</span></span>|<span data-ttu-id="20737-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="20737-153">DateTime the object was created.</span></span> <span data-ttu-id="20737-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20737-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20737-155">description</span><span class="sxs-lookup"><span data-stu-id="20737-155">description</span></span>|<span data-ttu-id="20737-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20737-156">String</span></span>|<span data-ttu-id="20737-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="20737-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20737-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20737-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20737-159">displayName</span><span class="sxs-lookup"><span data-stu-id="20737-159">displayName</span></span>|<span data-ttu-id="20737-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20737-160">String</span></span>|<span data-ttu-id="20737-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="20737-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20737-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20737-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20737-163">Version</span><span class="sxs-lookup"><span data-stu-id="20737-163">version</span></span>|<span data-ttu-id="20737-164">Int32</span><span class="sxs-lookup"><span data-stu-id="20737-164">Int32</span></span>|<span data-ttu-id="20737-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="20737-165">Version of the device configuration.</span></span> <span data-ttu-id="20737-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20737-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20737-167">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="20737-167">intendedPurpose</span></span>|[<span data-ttu-id="20737-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="20737-168">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="20737-169">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="20737-169">Not yet documented.</span></span> <span data-ttu-id="20737-170">Mögliche Werte: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="20737-170">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="20737-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="20737-171">Response</span></span>
<span data-ttu-id="20737-172">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="20737-172">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20737-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20737-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="20737-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20737-174">Request</span></span>
<span data-ttu-id="20737-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20737-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="20737-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="20737-176">Response</span></span>
<span data-ttu-id="20737-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20737-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```




