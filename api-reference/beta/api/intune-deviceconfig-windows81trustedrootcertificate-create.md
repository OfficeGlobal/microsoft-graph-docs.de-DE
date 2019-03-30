---
title: Windows81TrustedRootCertificate erstellen
description: Erstellen eines neuen windows81TrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24fa5a31a1750c5936b1821878ed8a6671ce2c9f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981664"
---
# <a name="create-windows81trustedrootcertificate"></a><span data-ttu-id="8d0d3-103">Windows81TrustedRootCertificate erstellen</span><span class="sxs-lookup"><span data-stu-id="8d0d3-103">Create windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="8d0d3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d0d3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d0d3-106">Erstellen eines neuen [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-106">Create a new [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d0d3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d0d3-107">Prerequisites</span></span>
<span data-ttu-id="8d0d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d0d3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d0d3-110">Permission type</span></span>|<span data-ttu-id="8d0d3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d0d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d0d3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d0d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d0d3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d0d3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d0d3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d0d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d0d3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d0d3-115">Not supported.</span></span>|
|<span data-ttu-id="8d0d3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d0d3-116">Application</span></span>|<span data-ttu-id="8d0d3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d0d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d0d3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d0d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="8d0d3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d0d3-119">Request headers</span></span>
|<span data-ttu-id="8d0d3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d0d3-120">Header</span></span>|<span data-ttu-id="8d0d3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8d0d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d0d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d0d3-122">Authorization</span></span>|<span data-ttu-id="8d0d3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d0d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d0d3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8d0d3-124">Accept</span></span>|<span data-ttu-id="8d0d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d0d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d0d3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d0d3-126">Request body</span></span>
<span data-ttu-id="8d0d3-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windows81TrustedRootCertificate-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-127">In the request body, supply a JSON representation for the windows81TrustedRootCertificate object.</span></span>

<span data-ttu-id="8d0d3-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows81TrustedRootCertificate erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-128">The following table shows the properties that are required when you create the windows81TrustedRootCertificate.</span></span>

|<span data-ttu-id="8d0d3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d0d3-129">Property</span></span>|<span data-ttu-id="8d0d3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8d0d3-130">Type</span></span>|<span data-ttu-id="8d0d3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d0d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d0d3-132">id</span><span class="sxs-lookup"><span data-stu-id="8d0d3-132">id</span></span>|<span data-ttu-id="8d0d3-133">String</span><span class="sxs-lookup"><span data-stu-id="8d0d3-133">String</span></span>|<span data-ttu-id="8d0d3-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8d0d3-134">Key of the entity.</span></span> <span data-ttu-id="8d0d3-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d0d3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d0d3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8d0d3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d0d3-137">DateTimeOffset</span></span>|<span data-ttu-id="8d0d3-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8d0d3-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d0d3-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="8d0d3-140">roleScopeTagIds</span></span>|<span data-ttu-id="8d0d3-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8d0d3-141">String collection</span></span>|<span data-ttu-id="8d0d3-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8d0d3-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d0d3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8d0d3-144">supportsScopeTags</span></span>|<span data-ttu-id="8d0d3-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8d0d3-145">Boolean</span></span>|<span data-ttu-id="8d0d3-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8d0d3-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8d0d3-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8d0d3-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-149">This property is read-only.</span></span> <span data-ttu-id="8d0d3-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d0d3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d0d3-151">createdDateTime</span></span>|<span data-ttu-id="8d0d3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d0d3-152">DateTimeOffset</span></span>|<span data-ttu-id="8d0d3-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-153">DateTime the object was created.</span></span> <span data-ttu-id="8d0d3-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d0d3-155">description</span><span class="sxs-lookup"><span data-stu-id="8d0d3-155">description</span></span>|<span data-ttu-id="8d0d3-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d0d3-156">String</span></span>|<span data-ttu-id="8d0d3-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d0d3-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d0d3-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8d0d3-159">displayName</span></span>|<span data-ttu-id="8d0d3-160">String</span><span class="sxs-lookup"><span data-stu-id="8d0d3-160">String</span></span>|<span data-ttu-id="8d0d3-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d0d3-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d0d3-163">Version</span><span class="sxs-lookup"><span data-stu-id="8d0d3-163">version</span></span>|<span data-ttu-id="8d0d3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8d0d3-164">Int32</span></span>|<span data-ttu-id="8d0d3-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-165">Version of the device configuration.</span></span> <span data-ttu-id="8d0d3-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d0d3-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8d0d3-167">trustedRootCertificate</span></span>|<span data-ttu-id="8d0d3-168">Binär</span><span class="sxs-lookup"><span data-stu-id="8d0d3-168">Binary</span></span>|<span data-ttu-id="8d0d3-169">Vertrauenswürdiges Stammzertifikat</span><span class="sxs-lookup"><span data-stu-id="8d0d3-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="8d0d3-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="8d0d3-170">certFileName</span></span>|<span data-ttu-id="8d0d3-171">String</span><span class="sxs-lookup"><span data-stu-id="8d0d3-171">String</span></span>|<span data-ttu-id="8d0d3-172">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-172">File name to display in UI.</span></span>|
|<span data-ttu-id="8d0d3-173">destinationStore</span><span class="sxs-lookup"><span data-stu-id="8d0d3-173">destinationStore</span></span>|[<span data-ttu-id="8d0d3-174">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="8d0d3-174">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="8d0d3-175">Speicherort des Zielspeichers für das vertrauenswürdige Stammzertifikat.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-175">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="8d0d3-176">Mögliche Werte sind: `computerCertStoreRoot`, `computerCertStoreIntermediate` und `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-176">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="8d0d3-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d0d3-177">Response</span></span>
<span data-ttu-id="8d0d3-178">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-178">If successful, this method returns a `201 Created` response code and a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d0d3-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d0d3-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d0d3-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d0d3-180">Request</span></span>
<span data-ttu-id="8d0d3-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
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

### <a name="response"></a><span data-ttu-id="8d0d3-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d0d3-182">Response</span></span>
<span data-ttu-id="8d0d3-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d0d3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




