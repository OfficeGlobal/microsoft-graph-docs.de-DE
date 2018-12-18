---
title: Erstellen von iosTrustedRootCertificate
description: Erstellen eines neuen IosTrustedRootCertificate-Objekts.
author: tfitzmac
ms.openlocfilehash: efb1a1107b2e7efcacb108ac3ccb1db9ad347c55
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305306"
---
# <a name="create-iostrustedrootcertificate"></a><span data-ttu-id="d4787-103">Erstellen von iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d4787-103">Create iosTrustedRootCertificate</span></span>

> <span data-ttu-id="d4787-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d4787-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4787-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4787-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4787-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d4787-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4787-107">Erstellen eines neuen [IosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4787-107">Create a new [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4787-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4787-108">Prerequisites</span></span>
<span data-ttu-id="d4787-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4787-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4787-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4787-111">Permission type</span></span>|<span data-ttu-id="d4787-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4787-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4787-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4787-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4787-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4787-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4787-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4787-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4787-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4787-116">Not supported.</span></span>|
|<span data-ttu-id="d4787-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4787-117">Application</span></span>|<span data-ttu-id="d4787-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4787-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4787-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4787-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="d4787-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4787-120">Request headers</span></span>
|<span data-ttu-id="d4787-121">Header</span><span class="sxs-lookup"><span data-stu-id="d4787-121">Header</span></span>|<span data-ttu-id="d4787-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d4787-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4787-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d4787-123">Authorization</span></span>|<span data-ttu-id="d4787-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4787-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4787-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4787-125">Accept</span></span>|<span data-ttu-id="d4787-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4787-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4787-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4787-127">Request body</span></span>
<span data-ttu-id="d4787-128">Geben Sie im Textkörper Anforderung für das Objekt IosTrustedRootCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d4787-128">In the request body, supply a JSON representation for the iosTrustedRootCertificate object.</span></span>

<span data-ttu-id="d4787-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosTrustedRootCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4787-129">The following table shows the properties that are required when you create the iosTrustedRootCertificate.</span></span>

|<span data-ttu-id="d4787-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4787-130">Property</span></span>|<span data-ttu-id="d4787-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d4787-131">Type</span></span>|<span data-ttu-id="d4787-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4787-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4787-133">id</span><span class="sxs-lookup"><span data-stu-id="d4787-133">id</span></span>|<span data-ttu-id="d4787-134">String</span><span class="sxs-lookup"><span data-stu-id="d4787-134">String</span></span>|<span data-ttu-id="d4787-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d4787-135">Key of the entity.</span></span> <span data-ttu-id="d4787-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4787-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4787-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4787-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d4787-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4787-138">DateTimeOffset</span></span>|<span data-ttu-id="d4787-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4787-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d4787-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4787-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4787-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4787-141">roleScopeTagIds</span></span>|<span data-ttu-id="d4787-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d4787-142">String collection</span></span>|<span data-ttu-id="d4787-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="d4787-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4787-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4787-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4787-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d4787-145">supportsScopeTags</span></span>|<span data-ttu-id="d4787-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d4787-146">Boolean</span></span>|<span data-ttu-id="d4787-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4787-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d4787-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="d4787-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d4787-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d4787-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d4787-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4787-150">This property is read-only.</span></span> <span data-ttu-id="d4787-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4787-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4787-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4787-152">createdDateTime</span></span>|<span data-ttu-id="d4787-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4787-153">DateTimeOffset</span></span>|<span data-ttu-id="d4787-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4787-154">DateTime the object was created.</span></span> <span data-ttu-id="d4787-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4787-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4787-156">description</span><span class="sxs-lookup"><span data-stu-id="d4787-156">description</span></span>|<span data-ttu-id="d4787-157">String</span><span class="sxs-lookup"><span data-stu-id="d4787-157">String</span></span>|<span data-ttu-id="d4787-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d4787-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4787-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4787-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4787-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d4787-160">displayName</span></span>|<span data-ttu-id="d4787-161">String</span><span class="sxs-lookup"><span data-stu-id="d4787-161">String</span></span>|<span data-ttu-id="d4787-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d4787-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4787-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4787-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4787-164">Version</span><span class="sxs-lookup"><span data-stu-id="d4787-164">version</span></span>|<span data-ttu-id="d4787-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d4787-165">Int32</span></span>|<span data-ttu-id="d4787-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d4787-166">Version of the device configuration.</span></span> <span data-ttu-id="d4787-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4787-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4787-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d4787-168">trustedRootCertificate</span></span>|<span data-ttu-id="d4787-169">Binär</span><span class="sxs-lookup"><span data-stu-id="d4787-169">Binary</span></span>|<span data-ttu-id="d4787-170">Zertifikat der vertrauenswürdigen Stammzertifizierungsstellen.</span><span class="sxs-lookup"><span data-stu-id="d4787-170">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="d4787-171">Aus</span><span class="sxs-lookup"><span data-stu-id="d4787-171">certFileName</span></span>|<span data-ttu-id="d4787-172">String</span><span class="sxs-lookup"><span data-stu-id="d4787-172">String</span></span>|<span data-ttu-id="d4787-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d4787-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="d4787-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4787-174">Response</span></span>
<span data-ttu-id="d4787-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d4787-175">If successful, this method returns a `201 Created` response code and a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4787-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4787-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4787-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4787-177">Request</span></span>
<span data-ttu-id="d4787-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4787-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
Content-type: application/json
Content-length: 427

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="d4787-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4787-179">Response</span></span>
<span data-ttu-id="d4787-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4787-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





