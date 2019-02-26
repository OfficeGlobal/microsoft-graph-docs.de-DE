---
title: IosTrustedRootCertificate aktualisieren
description: Aktualisieren der Eigenschaften eines iosTrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2436cd551e2e84e128b620d4ff2d06a28a0670a4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165639"
---
# <a name="update-iostrustedrootcertificate"></a><span data-ttu-id="4812c-103">IosTrustedRootCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4812c-103">Update iosTrustedRootCertificate</span></span>

> <span data-ttu-id="4812c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4812c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4812c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4812c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4812c-106">Aktualisieren der Eigenschaften eines [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4812c-106">Update the properties of a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4812c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4812c-107">Prerequisites</span></span>
<span data-ttu-id="4812c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4812c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4812c-110">Permission type</span></span>|<span data-ttu-id="4812c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4812c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4812c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4812c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4812c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4812c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4812c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4812c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4812c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4812c-115">Not supported.</span></span>|
|<span data-ttu-id="4812c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4812c-116">Application</span></span>|<span data-ttu-id="4812c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4812c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4812c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4812c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{iosTrustedRootCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="4812c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4812c-119">Request headers</span></span>
|<span data-ttu-id="4812c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4812c-120">Header</span></span>|<span data-ttu-id="4812c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4812c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4812c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4812c-122">Authorization</span></span>|<span data-ttu-id="4812c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4812c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4812c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4812c-124">Accept</span></span>|<span data-ttu-id="4812c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4812c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4812c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4812c-126">Request body</span></span>
<span data-ttu-id="4812c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4812c-127">In the request body, supply a JSON representation for the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="4812c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4812c-128">The following table shows the properties that are required when you create the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="4812c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4812c-129">Property</span></span>|<span data-ttu-id="4812c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4812c-130">Type</span></span>|<span data-ttu-id="4812c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4812c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4812c-132">id</span><span class="sxs-lookup"><span data-stu-id="4812c-132">id</span></span>|<span data-ttu-id="4812c-133">string</span><span class="sxs-lookup"><span data-stu-id="4812c-133">String</span></span>|<span data-ttu-id="4812c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4812c-134">Key of the entity.</span></span> <span data-ttu-id="4812c-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4812c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4812c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4812c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4812c-137">DateTimeOffset</span></span>|<span data-ttu-id="4812c-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4812c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4812c-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4812c-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="4812c-140">roleScopeTagIds</span></span>|<span data-ttu-id="4812c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4812c-141">String collection</span></span>|<span data-ttu-id="4812c-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="4812c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4812c-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4812c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4812c-144">supportsScopeTags</span></span>|<span data-ttu-id="4812c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4812c-145">Boolean</span></span>|<span data-ttu-id="4812c-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4812c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4812c-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="4812c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4812c-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="4812c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4812c-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4812c-149">This property is read-only.</span></span> <span data-ttu-id="4812c-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4812c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4812c-151">createdDateTime</span></span>|<span data-ttu-id="4812c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4812c-152">DateTimeOffset</span></span>|<span data-ttu-id="4812c-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4812c-153">DateTime the object was created.</span></span> <span data-ttu-id="4812c-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4812c-155">description</span><span class="sxs-lookup"><span data-stu-id="4812c-155">description</span></span>|<span data-ttu-id="4812c-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4812c-156">String</span></span>|<span data-ttu-id="4812c-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4812c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4812c-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4812c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4812c-159">displayName</span></span>|<span data-ttu-id="4812c-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4812c-160">String</span></span>|<span data-ttu-id="4812c-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4812c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4812c-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4812c-163">Version</span><span class="sxs-lookup"><span data-stu-id="4812c-163">version</span></span>|<span data-ttu-id="4812c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4812c-164">Int32</span></span>|<span data-ttu-id="4812c-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4812c-165">Version of the device configuration.</span></span> <span data-ttu-id="4812c-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4812c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4812c-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="4812c-167">trustedRootCertificate</span></span>|<span data-ttu-id="4812c-168">Binär</span><span class="sxs-lookup"><span data-stu-id="4812c-168">Binary</span></span>|<span data-ttu-id="4812c-169">Vertrauenswürdiges Stammzertifikat.</span><span class="sxs-lookup"><span data-stu-id="4812c-169">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="4812c-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="4812c-170">certFileName</span></span>|<span data-ttu-id="4812c-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4812c-171">String</span></span>|<span data-ttu-id="4812c-172">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="4812c-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="4812c-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="4812c-173">Response</span></span>
<span data-ttu-id="4812c-174">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4812c-174">If successful, this method returns a `200 OK` response code and an updated [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4812c-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4812c-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="4812c-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4812c-176">Request</span></span>
<span data-ttu-id="4812c-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4812c-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="4812c-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="4812c-178">Response</span></span>
<span data-ttu-id="4812c-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4812c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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




