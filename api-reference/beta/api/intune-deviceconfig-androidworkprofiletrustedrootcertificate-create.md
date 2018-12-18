---
title: Erstellen von androidWorkProfileTrustedRootCertificate
description: Erstellen eines neuen AndroidWorkProfileTrustedRootCertificate-Objekts.
author: tfitzmac
ms.openlocfilehash: e48e1ea77c09e9b0b53883ac68707c5a1ab2efd1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360032"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="8ebf4-103">Erstellen von androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8ebf4-103">Create androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="8ebf4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ebf4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ebf4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ebf4-107">Erstellen eines neuen [AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-107">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ebf4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8ebf4-108">Prerequisites</span></span>
<span data-ttu-id="8ebf4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ebf4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ebf4-111">Permission type</span></span>|<span data-ttu-id="8ebf4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ebf4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ebf4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ebf4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ebf4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ebf4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ebf4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ebf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ebf4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ebf4-116">Not supported.</span></span>|
|<span data-ttu-id="8ebf4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ebf4-117">Application</span></span>|<span data-ttu-id="8ebf4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ebf4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ebf4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ebf4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8ebf4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ebf4-120">Request headers</span></span>
|<span data-ttu-id="8ebf4-121">Header</span><span class="sxs-lookup"><span data-stu-id="8ebf4-121">Header</span></span>|<span data-ttu-id="8ebf4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8ebf4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ebf4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8ebf4-123">Authorization</span></span>|<span data-ttu-id="8ebf4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8ebf4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ebf4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ebf4-125">Accept</span></span>|<span data-ttu-id="8ebf4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ebf4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ebf4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ebf4-127">Request body</span></span>
<span data-ttu-id="8ebf4-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileTrustedRootCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-128">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="8ebf4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileTrustedRootCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-129">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="8ebf4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8ebf4-130">Property</span></span>|<span data-ttu-id="8ebf4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8ebf4-131">Type</span></span>|<span data-ttu-id="8ebf4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ebf4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ebf4-133">id</span><span class="sxs-lookup"><span data-stu-id="8ebf4-133">id</span></span>|<span data-ttu-id="8ebf4-134">String</span><span class="sxs-lookup"><span data-stu-id="8ebf4-134">String</span></span>|<span data-ttu-id="8ebf4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8ebf4-135">Key of the entity.</span></span> <span data-ttu-id="8ebf4-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ebf4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ebf4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8ebf4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ebf4-138">DateTimeOffset</span></span>|<span data-ttu-id="8ebf4-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8ebf4-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ebf4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ebf4-141">roleScopeTagIds</span></span>|<span data-ttu-id="8ebf4-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="8ebf4-142">String collection</span></span>|<span data-ttu-id="8ebf4-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ebf4-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ebf4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8ebf4-145">supportsScopeTags</span></span>|<span data-ttu-id="8ebf4-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8ebf4-146">Boolean</span></span>|<span data-ttu-id="8ebf4-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ebf4-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ebf4-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ebf4-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-150">This property is read-only.</span></span> <span data-ttu-id="8ebf4-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ebf4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ebf4-152">createdDateTime</span></span>|<span data-ttu-id="8ebf4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ebf4-153">DateTimeOffset</span></span>|<span data-ttu-id="8ebf4-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-154">DateTime the object was created.</span></span> <span data-ttu-id="8ebf4-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ebf4-156">description</span><span class="sxs-lookup"><span data-stu-id="8ebf4-156">description</span></span>|<span data-ttu-id="8ebf4-157">String</span><span class="sxs-lookup"><span data-stu-id="8ebf4-157">String</span></span>|<span data-ttu-id="8ebf4-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ebf4-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ebf4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8ebf4-160">displayName</span></span>|<span data-ttu-id="8ebf4-161">String</span><span class="sxs-lookup"><span data-stu-id="8ebf4-161">String</span></span>|<span data-ttu-id="8ebf4-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ebf4-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ebf4-164">Version</span><span class="sxs-lookup"><span data-stu-id="8ebf4-164">version</span></span>|<span data-ttu-id="8ebf4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8ebf4-165">Int32</span></span>|<span data-ttu-id="8ebf4-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-166">Version of the device configuration.</span></span> <span data-ttu-id="8ebf4-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ebf4-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8ebf4-168">trustedRootCertificate</span></span>|<span data-ttu-id="8ebf4-169">Binär</span><span class="sxs-lookup"><span data-stu-id="8ebf4-169">Binary</span></span>|<span data-ttu-id="8ebf4-170">Vertrauenswürdiges Zertifikat</span><span class="sxs-lookup"><span data-stu-id="8ebf4-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="8ebf4-171">Aus</span><span class="sxs-lookup"><span data-stu-id="8ebf4-171">certFileName</span></span>|<span data-ttu-id="8ebf4-172">String</span><span class="sxs-lookup"><span data-stu-id="8ebf4-172">String</span></span>|<span data-ttu-id="8ebf4-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="8ebf4-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ebf4-174">Response</span></span>
<span data-ttu-id="8ebf4-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-175">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ebf4-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ebf4-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ebf4-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ebf4-177">Request</span></span>
<span data-ttu-id="8ebf4-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 442

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="8ebf4-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ebf4-179">Response</span></span>
<span data-ttu-id="8ebf4-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





