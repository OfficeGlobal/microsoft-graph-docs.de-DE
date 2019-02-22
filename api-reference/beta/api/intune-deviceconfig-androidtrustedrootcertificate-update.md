---
title: AndroidTrustedRootCertificate aktualisieren
description: Aktualisieren der Eigenschaften eines androidTrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74cab640907c5dc4c96697fce5f77258af742ca1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155013"
---
# <a name="update-androidtrustedrootcertificate"></a><span data-ttu-id="fff47-103">AndroidTrustedRootCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fff47-103">Update androidTrustedRootCertificate</span></span>

> <span data-ttu-id="fff47-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fff47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fff47-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fff47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fff47-106">Aktualisieren der Eigenschaften eines [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fff47-106">Update the properties of a [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fff47-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fff47-107">Prerequisites</span></span>
<span data-ttu-id="fff47-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fff47-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fff47-110">Permission type</span></span>|<span data-ttu-id="fff47-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fff47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fff47-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fff47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fff47-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fff47-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fff47-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fff47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fff47-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fff47-115">Not supported.</span></span>|
|<span data-ttu-id="fff47-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fff47-116">Application</span></span>|<span data-ttu-id="fff47-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fff47-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fff47-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fff47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="fff47-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fff47-119">Request headers</span></span>
|<span data-ttu-id="fff47-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fff47-120">Header</span></span>|<span data-ttu-id="fff47-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fff47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fff47-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fff47-122">Authorization</span></span>|<span data-ttu-id="fff47-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fff47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fff47-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fff47-124">Accept</span></span>|<span data-ttu-id="fff47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fff47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fff47-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fff47-126">Request body</span></span>
<span data-ttu-id="fff47-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="fff47-127">In the request body, supply a JSON representation for the [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="fff47-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fff47-128">The following table shows the properties that are required when you create the [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md).</span></span>

|<span data-ttu-id="fff47-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fff47-129">Property</span></span>|<span data-ttu-id="fff47-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fff47-130">Type</span></span>|<span data-ttu-id="fff47-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fff47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fff47-132">id</span><span class="sxs-lookup"><span data-stu-id="fff47-132">id</span></span>|<span data-ttu-id="fff47-133">string</span><span class="sxs-lookup"><span data-stu-id="fff47-133">String</span></span>|<span data-ttu-id="fff47-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fff47-134">Key of the entity.</span></span> <span data-ttu-id="fff47-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fff47-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fff47-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fff47-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fff47-137">DateTimeOffset</span></span>|<span data-ttu-id="fff47-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fff47-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fff47-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fff47-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="fff47-140">roleScopeTagIds</span></span>|<span data-ttu-id="fff47-141">String collection</span><span class="sxs-lookup"><span data-stu-id="fff47-141">String collection</span></span>|<span data-ttu-id="fff47-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="fff47-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fff47-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fff47-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fff47-144">supportsScopeTags</span></span>|<span data-ttu-id="fff47-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fff47-145">Boolean</span></span>|<span data-ttu-id="fff47-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fff47-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fff47-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="fff47-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fff47-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="fff47-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fff47-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fff47-149">This property is read-only.</span></span> <span data-ttu-id="fff47-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fff47-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fff47-151">createdDateTime</span></span>|<span data-ttu-id="fff47-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fff47-152">DateTimeOffset</span></span>|<span data-ttu-id="fff47-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fff47-153">DateTime the object was created.</span></span> <span data-ttu-id="fff47-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fff47-155">description</span><span class="sxs-lookup"><span data-stu-id="fff47-155">description</span></span>|<span data-ttu-id="fff47-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fff47-156">String</span></span>|<span data-ttu-id="fff47-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fff47-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fff47-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fff47-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fff47-159">displayName</span></span>|<span data-ttu-id="fff47-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fff47-160">String</span></span>|<span data-ttu-id="fff47-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fff47-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fff47-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fff47-163">Version</span><span class="sxs-lookup"><span data-stu-id="fff47-163">version</span></span>|<span data-ttu-id="fff47-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fff47-164">Int32</span></span>|<span data-ttu-id="fff47-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="fff47-165">Version of the device configuration.</span></span> <span data-ttu-id="fff47-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fff47-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fff47-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fff47-167">trustedRootCertificate</span></span>|<span data-ttu-id="fff47-168">Binär</span><span class="sxs-lookup"><span data-stu-id="fff47-168">Binary</span></span>|<span data-ttu-id="fff47-169">Vertrauenswürdiges Stammzertifikat</span><span class="sxs-lookup"><span data-stu-id="fff47-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="fff47-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="fff47-170">certFileName</span></span>|<span data-ttu-id="fff47-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fff47-171">String</span></span>|<span data-ttu-id="fff47-172">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="fff47-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="fff47-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="fff47-173">Response</span></span>
<span data-ttu-id="fff47-174">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fff47-174">If successful, this method returns a `200 OK` response code and an updated [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fff47-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fff47-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="fff47-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fff47-176">Request</span></span>
<span data-ttu-id="fff47-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fff47-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 367

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="fff47-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="fff47-178">Response</span></span>
<span data-ttu-id="fff47-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fff47-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
  "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
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




