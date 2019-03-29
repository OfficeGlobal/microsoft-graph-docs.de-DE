---
title: Windows81TrustedRootCertificate aktualisieren
description: Aktualisieren der Eigenschaften eines windows81TrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0950f44708ba46b851203673ba7c1c5c6c269f6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964304"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="9ead0-103">Windows81TrustedRootCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9ead0-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="9ead0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ead0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ead0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9ead0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ead0-106">Aktualisieren der Eigenschaften eines [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ead0-106">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ead0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ead0-107">Prerequisites</span></span>
<span data-ttu-id="9ead0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ead0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ead0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ead0-110">Permission type</span></span>|<span data-ttu-id="9ead0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ead0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ead0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ead0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ead0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ead0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ead0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ead0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ead0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ead0-115">Not supported.</span></span>|
|<span data-ttu-id="9ead0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ead0-116">Application</span></span>|<span data-ttu-id="9ead0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ead0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ead0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ead0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="9ead0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ead0-119">Request headers</span></span>
|<span data-ttu-id="9ead0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9ead0-120">Header</span></span>|<span data-ttu-id="9ead0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9ead0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ead0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ead0-122">Authorization</span></span>|<span data-ttu-id="9ead0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ead0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ead0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9ead0-124">Accept</span></span>|<span data-ttu-id="9ead0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ead0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ead0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ead0-126">Request body</span></span>
<span data-ttu-id="9ead0-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="9ead0-127">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="9ead0-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9ead0-128">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="9ead0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ead0-129">Property</span></span>|<span data-ttu-id="9ead0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9ead0-130">Type</span></span>|<span data-ttu-id="9ead0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ead0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ead0-132">id</span><span class="sxs-lookup"><span data-stu-id="9ead0-132">id</span></span>|<span data-ttu-id="9ead0-133">String</span><span class="sxs-lookup"><span data-stu-id="9ead0-133">String</span></span>|<span data-ttu-id="9ead0-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9ead0-134">Key of the entity.</span></span> <span data-ttu-id="9ead0-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ead0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ead0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9ead0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ead0-137">DateTimeOffset</span></span>|<span data-ttu-id="9ead0-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ead0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9ead0-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ead0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead0-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="9ead0-140">roleScopeTagIds</span></span>|<span data-ttu-id="9ead0-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9ead0-141">String collection</span></span>|<span data-ttu-id="9ead0-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="9ead0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ead0-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ead0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ead0-144">supportsScopeTags</span></span>|<span data-ttu-id="9ead0-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9ead0-145">Boolean</span></span>|<span data-ttu-id="9ead0-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ead0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ead0-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="9ead0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ead0-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="9ead0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ead0-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9ead0-149">This property is read-only.</span></span> <span data-ttu-id="9ead0-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ead0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ead0-151">createdDateTime</span></span>|<span data-ttu-id="9ead0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ead0-152">DateTimeOffset</span></span>|<span data-ttu-id="9ead0-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ead0-153">DateTime the object was created.</span></span> <span data-ttu-id="9ead0-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ead0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead0-155">description</span><span class="sxs-lookup"><span data-stu-id="9ead0-155">description</span></span>|<span data-ttu-id="9ead0-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ead0-156">String</span></span>|<span data-ttu-id="9ead0-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9ead0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ead0-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ead0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9ead0-159">displayName</span></span>|<span data-ttu-id="9ead0-160">String</span><span class="sxs-lookup"><span data-stu-id="9ead0-160">String</span></span>|<span data-ttu-id="9ead0-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9ead0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ead0-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ead0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead0-163">Version</span><span class="sxs-lookup"><span data-stu-id="9ead0-163">version</span></span>|<span data-ttu-id="9ead0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9ead0-164">Int32</span></span>|<span data-ttu-id="9ead0-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9ead0-165">Version of the device configuration.</span></span> <span data-ttu-id="9ead0-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ead0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead0-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9ead0-167">trustedRootCertificate</span></span>|<span data-ttu-id="9ead0-168">Binär</span><span class="sxs-lookup"><span data-stu-id="9ead0-168">Binary</span></span>|<span data-ttu-id="9ead0-169">Vertrauenswürdiges Stammzertifikat</span><span class="sxs-lookup"><span data-stu-id="9ead0-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="9ead0-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="9ead0-170">certFileName</span></span>|<span data-ttu-id="9ead0-171">String</span><span class="sxs-lookup"><span data-stu-id="9ead0-171">String</span></span>|<span data-ttu-id="9ead0-172">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9ead0-172">File name to display in UI.</span></span>|
|<span data-ttu-id="9ead0-173">destinationStore</span><span class="sxs-lookup"><span data-stu-id="9ead0-173">destinationStore</span></span>|[<span data-ttu-id="9ead0-174">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="9ead0-174">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="9ead0-175">Speicherort des Zielspeichers für das vertrauenswürdige Stammzertifikat.</span><span class="sxs-lookup"><span data-stu-id="9ead0-175">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="9ead0-176">Mögliche Werte sind: `computerCertStoreRoot`, `computerCertStoreIntermediate` und `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="9ead0-176">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="9ead0-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ead0-177">Response</span></span>
<span data-ttu-id="9ead0-178">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9ead0-178">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ead0-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ead0-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ead0-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ead0-180">Request</span></span>
<span data-ttu-id="9ead0-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ead0-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="9ead0-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ead0-182">Response</span></span>
<span data-ttu-id="9ead0-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ead0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 597

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




