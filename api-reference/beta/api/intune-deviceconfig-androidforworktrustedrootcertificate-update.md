---
title: AndroidForWorkTrustedRootCertificate aktualisieren
description: Aktualisieren der Eigenschaften eines androidForWorkTrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61da2ce8bf9a73f2121ceaaed315e6347bd6cd9c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980327"
---
# <a name="update-androidforworktrustedrootcertificate"></a><span data-ttu-id="9a3d6-103">AndroidForWorkTrustedRootCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9a3d6-103">Update androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="9a3d6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a3d6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a3d6-106">Aktualisieren der Eigenschaften eines [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-106">Update the properties of a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a3d6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9a3d6-107">Prerequisites</span></span>
<span data-ttu-id="9a3d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a3d6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a3d6-110">Permission type</span></span>|<span data-ttu-id="9a3d6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a3d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a3d6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a3d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a3d6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a3d6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a3d6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a3d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a3d6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a3d6-115">Not supported.</span></span>|
|<span data-ttu-id="9a3d6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a3d6-116">Application</span></span>|<span data-ttu-id="9a3d6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a3d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a3d6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a3d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="9a3d6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a3d6-119">Request headers</span></span>
|<span data-ttu-id="9a3d6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9a3d6-120">Header</span></span>|<span data-ttu-id="9a3d6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9a3d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a3d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a3d6-122">Authorization</span></span>|<span data-ttu-id="9a3d6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9a3d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a3d6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9a3d6-124">Accept</span></span>|<span data-ttu-id="9a3d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9a3d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a3d6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a3d6-126">Request body</span></span>
<span data-ttu-id="9a3d6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-127">In the request body, supply a JSON representation for the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="9a3d6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-128">The following table shows the properties that are required when you create the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span></span>

|<span data-ttu-id="9a3d6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9a3d6-129">Property</span></span>|<span data-ttu-id="9a3d6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9a3d6-130">Type</span></span>|<span data-ttu-id="9a3d6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a3d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a3d6-132">id</span><span class="sxs-lookup"><span data-stu-id="9a3d6-132">id</span></span>|<span data-ttu-id="9a3d6-133">String</span><span class="sxs-lookup"><span data-stu-id="9a3d6-133">String</span></span>|<span data-ttu-id="9a3d6-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9a3d6-134">Key of the entity.</span></span> <span data-ttu-id="9a3d6-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a3d6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a3d6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9a3d6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a3d6-137">DateTimeOffset</span></span>|<span data-ttu-id="9a3d6-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9a3d6-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a3d6-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="9a3d6-140">roleScopeTagIds</span></span>|<span data-ttu-id="9a3d6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9a3d6-141">String collection</span></span>|<span data-ttu-id="9a3d6-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a3d6-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a3d6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9a3d6-144">supportsScopeTags</span></span>|<span data-ttu-id="9a3d6-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9a3d6-145">Boolean</span></span>|<span data-ttu-id="9a3d6-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9a3d6-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9a3d6-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9a3d6-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-149">This property is read-only.</span></span> <span data-ttu-id="9a3d6-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a3d6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a3d6-151">createdDateTime</span></span>|<span data-ttu-id="9a3d6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a3d6-152">DateTimeOffset</span></span>|<span data-ttu-id="9a3d6-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-153">DateTime the object was created.</span></span> <span data-ttu-id="9a3d6-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a3d6-155">description</span><span class="sxs-lookup"><span data-stu-id="9a3d6-155">description</span></span>|<span data-ttu-id="9a3d6-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a3d6-156">String</span></span>|<span data-ttu-id="9a3d6-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a3d6-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a3d6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9a3d6-159">displayName</span></span>|<span data-ttu-id="9a3d6-160">String</span><span class="sxs-lookup"><span data-stu-id="9a3d6-160">String</span></span>|<span data-ttu-id="9a3d6-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a3d6-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a3d6-163">Version</span><span class="sxs-lookup"><span data-stu-id="9a3d6-163">version</span></span>|<span data-ttu-id="9a3d6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9a3d6-164">Int32</span></span>|<span data-ttu-id="9a3d6-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-165">Version of the device configuration.</span></span> <span data-ttu-id="9a3d6-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a3d6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a3d6-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a3d6-167">trustedRootCertificate</span></span>|<span data-ttu-id="9a3d6-168">Binär</span><span class="sxs-lookup"><span data-stu-id="9a3d6-168">Binary</span></span>|<span data-ttu-id="9a3d6-169">Vertrauenswürdiges Stammzertifikat</span><span class="sxs-lookup"><span data-stu-id="9a3d6-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="9a3d6-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="9a3d6-170">certFileName</span></span>|<span data-ttu-id="9a3d6-171">String</span><span class="sxs-lookup"><span data-stu-id="9a3d6-171">String</span></span>|<span data-ttu-id="9a3d6-172">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="9a3d6-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a3d6-173">Response</span></span>
<span data-ttu-id="9a3d6-174">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-174">If successful, this method returns a `200 OK` response code and an updated [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a3d6-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a3d6-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a3d6-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a3d6-176">Request</span></span>
<span data-ttu-id="9a3d6-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="9a3d6-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a3d6-178">Response</span></span>
<span data-ttu-id="9a3d6-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a3d6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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




