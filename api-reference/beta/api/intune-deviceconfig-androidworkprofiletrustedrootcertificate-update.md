---
title: AndroidWorkProfileTrustedRootCertificate aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidWorkProfileTrustedRootCertificate-Objekts.
author: tfitzmac
ms.openlocfilehash: 1078a0724908c7b28845303a1392f19c27ab9a42
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341293"
---
# <a name="update-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="8eb12-103">AndroidWorkProfileTrustedRootCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8eb12-103">Update androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="8eb12-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8eb12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eb12-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8eb12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8eb12-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8eb12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8eb12-107">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8eb12-107">Update the properties of a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8eb12-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8eb12-108">Prerequisites</span></span>
<span data-ttu-id="8eb12-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eb12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eb12-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8eb12-111">Permission type</span></span>|<span data-ttu-id="8eb12-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8eb12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eb12-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8eb12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8eb12-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb12-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8eb12-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8eb12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eb12-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8eb12-116">Not supported.</span></span>|
|<span data-ttu-id="8eb12-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8eb12-117">Application</span></span>|<span data-ttu-id="8eb12-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8eb12-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eb12-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8eb12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="8eb12-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8eb12-120">Request headers</span></span>
|<span data-ttu-id="8eb12-121">Header</span><span class="sxs-lookup"><span data-stu-id="8eb12-121">Header</span></span>|<span data-ttu-id="8eb12-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8eb12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eb12-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8eb12-123">Authorization</span></span>|<span data-ttu-id="8eb12-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8eb12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eb12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8eb12-125">Accept</span></span>|<span data-ttu-id="8eb12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8eb12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eb12-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8eb12-127">Request body</span></span>
<span data-ttu-id="8eb12-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8eb12-128">In the request body, supply a JSON representation for the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="8eb12-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="8eb12-129">The following table shows the properties that are required when you create the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span></span>

|<span data-ttu-id="8eb12-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8eb12-130">Property</span></span>|<span data-ttu-id="8eb12-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8eb12-131">Type</span></span>|<span data-ttu-id="8eb12-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8eb12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb12-133">id</span><span class="sxs-lookup"><span data-stu-id="8eb12-133">id</span></span>|<span data-ttu-id="8eb12-134">String</span><span class="sxs-lookup"><span data-stu-id="8eb12-134">String</span></span>|<span data-ttu-id="8eb12-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8eb12-135">Key of the entity.</span></span> <span data-ttu-id="8eb12-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb12-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb12-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8eb12-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8eb12-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eb12-138">DateTimeOffset</span></span>|<span data-ttu-id="8eb12-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8eb12-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8eb12-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb12-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb12-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8eb12-141">roleScopeTagIds</span></span>|<span data-ttu-id="8eb12-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="8eb12-142">String collection</span></span>|<span data-ttu-id="8eb12-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="8eb12-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8eb12-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb12-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb12-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8eb12-145">supportsScopeTags</span></span>|<span data-ttu-id="8eb12-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8eb12-146">Boolean</span></span>|<span data-ttu-id="8eb12-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8eb12-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8eb12-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="8eb12-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8eb12-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="8eb12-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8eb12-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8eb12-150">This property is read-only.</span></span> <span data-ttu-id="8eb12-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb12-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb12-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8eb12-152">createdDateTime</span></span>|<span data-ttu-id="8eb12-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eb12-153">DateTimeOffset</span></span>|<span data-ttu-id="8eb12-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8eb12-154">DateTime the object was created.</span></span> <span data-ttu-id="8eb12-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb12-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb12-156">description</span><span class="sxs-lookup"><span data-stu-id="8eb12-156">description</span></span>|<span data-ttu-id="8eb12-157">String</span><span class="sxs-lookup"><span data-stu-id="8eb12-157">String</span></span>|<span data-ttu-id="8eb12-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8eb12-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8eb12-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb12-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb12-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8eb12-160">displayName</span></span>|<span data-ttu-id="8eb12-161">String</span><span class="sxs-lookup"><span data-stu-id="8eb12-161">String</span></span>|<span data-ttu-id="8eb12-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8eb12-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8eb12-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb12-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb12-164">Version</span><span class="sxs-lookup"><span data-stu-id="8eb12-164">version</span></span>|<span data-ttu-id="8eb12-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8eb12-165">Int32</span></span>|<span data-ttu-id="8eb12-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8eb12-166">Version of the device configuration.</span></span> <span data-ttu-id="8eb12-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb12-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb12-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8eb12-168">trustedRootCertificate</span></span>|<span data-ttu-id="8eb12-169">Binär</span><span class="sxs-lookup"><span data-stu-id="8eb12-169">Binary</span></span>|<span data-ttu-id="8eb12-170">Vertrauenswürdiges Zertifikat</span><span class="sxs-lookup"><span data-stu-id="8eb12-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="8eb12-171">Aus</span><span class="sxs-lookup"><span data-stu-id="8eb12-171">certFileName</span></span>|<span data-ttu-id="8eb12-172">String</span><span class="sxs-lookup"><span data-stu-id="8eb12-172">String</span></span>|<span data-ttu-id="8eb12-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8eb12-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="8eb12-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="8eb12-174">Response</span></span>
<span data-ttu-id="8eb12-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8eb12-175">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eb12-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8eb12-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8eb12-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8eb12-177">Request</span></span>
<span data-ttu-id="8eb12-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8eb12-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 363

{
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

### <a name="response"></a><span data-ttu-id="8eb12-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="8eb12-179">Response</span></span>
<span data-ttu-id="8eb12-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8eb12-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





