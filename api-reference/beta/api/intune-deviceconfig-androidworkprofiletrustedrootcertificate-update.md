---
title: AndroidWorkProfileTrustedRootCertificate aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileTrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba4c3b324f451bc6d839711c52f5c9bc135bc567
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967055"
---
# <a name="update-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="28db4-103">AndroidWorkProfileTrustedRootCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="28db4-103">Update androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="28db4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28db4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28db4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="28db4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28db4-106">Aktualisieren der Eigenschaften eines [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="28db4-106">Update the properties of a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28db4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28db4-107">Prerequisites</span></span>
<span data-ttu-id="28db4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28db4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28db4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28db4-110">Permission type</span></span>|<span data-ttu-id="28db4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28db4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28db4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28db4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28db4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28db4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28db4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28db4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28db4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28db4-115">Not supported.</span></span>|
|<span data-ttu-id="28db4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28db4-116">Application</span></span>|<span data-ttu-id="28db4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28db4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28db4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28db4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="28db4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28db4-119">Request headers</span></span>
|<span data-ttu-id="28db4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="28db4-120">Header</span></span>|<span data-ttu-id="28db4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="28db4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28db4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28db4-122">Authorization</span></span>|<span data-ttu-id="28db4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28db4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28db4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="28db4-124">Accept</span></span>|<span data-ttu-id="28db4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28db4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28db4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28db4-126">Request body</span></span>
<span data-ttu-id="28db4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="28db4-127">In the request body, supply a JSON representation for the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="28db4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="28db4-128">The following table shows the properties that are required when you create the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span></span>

|<span data-ttu-id="28db4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28db4-129">Property</span></span>|<span data-ttu-id="28db4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="28db4-130">Type</span></span>|<span data-ttu-id="28db4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28db4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28db4-132">id</span><span class="sxs-lookup"><span data-stu-id="28db4-132">id</span></span>|<span data-ttu-id="28db4-133">String</span><span class="sxs-lookup"><span data-stu-id="28db4-133">String</span></span>|<span data-ttu-id="28db4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="28db4-134">Key of the entity.</span></span> <span data-ttu-id="28db4-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28db4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28db4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28db4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="28db4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28db4-137">DateTimeOffset</span></span>|<span data-ttu-id="28db4-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="28db4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="28db4-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28db4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28db4-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="28db4-140">roleScopeTagIds</span></span>|<span data-ttu-id="28db4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="28db4-141">String collection</span></span>|<span data-ttu-id="28db4-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="28db4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="28db4-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28db4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28db4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="28db4-144">supportsScopeTags</span></span>|<span data-ttu-id="28db4-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="28db4-145">Boolean</span></span>|<span data-ttu-id="28db4-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28db4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="28db4-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="28db4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="28db4-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="28db4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="28db4-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="28db4-149">This property is read-only.</span></span> <span data-ttu-id="28db4-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28db4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28db4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28db4-151">createdDateTime</span></span>|<span data-ttu-id="28db4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28db4-152">DateTimeOffset</span></span>|<span data-ttu-id="28db4-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="28db4-153">DateTime the object was created.</span></span> <span data-ttu-id="28db4-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28db4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28db4-155">description</span><span class="sxs-lookup"><span data-stu-id="28db4-155">description</span></span>|<span data-ttu-id="28db4-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28db4-156">String</span></span>|<span data-ttu-id="28db4-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="28db4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="28db4-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28db4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28db4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="28db4-159">displayName</span></span>|<span data-ttu-id="28db4-160">String</span><span class="sxs-lookup"><span data-stu-id="28db4-160">String</span></span>|<span data-ttu-id="28db4-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="28db4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="28db4-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28db4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28db4-163">Version</span><span class="sxs-lookup"><span data-stu-id="28db4-163">version</span></span>|<span data-ttu-id="28db4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="28db4-164">Int32</span></span>|<span data-ttu-id="28db4-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="28db4-165">Version of the device configuration.</span></span> <span data-ttu-id="28db4-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28db4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28db4-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="28db4-167">trustedRootCertificate</span></span>|<span data-ttu-id="28db4-168">Binär</span><span class="sxs-lookup"><span data-stu-id="28db4-168">Binary</span></span>|<span data-ttu-id="28db4-169">Vertrauenswürdiges Stammzertifikat</span><span class="sxs-lookup"><span data-stu-id="28db4-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="28db4-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="28db4-170">certFileName</span></span>|<span data-ttu-id="28db4-171">String</span><span class="sxs-lookup"><span data-stu-id="28db4-171">String</span></span>|<span data-ttu-id="28db4-172">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="28db4-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="28db4-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="28db4-173">Response</span></span>
<span data-ttu-id="28db4-174">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="28db4-174">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28db4-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28db4-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="28db4-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28db4-176">Request</span></span>
<span data-ttu-id="28db4-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28db4-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="28db4-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="28db4-178">Response</span></span>
<span data-ttu-id="28db4-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28db4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```




