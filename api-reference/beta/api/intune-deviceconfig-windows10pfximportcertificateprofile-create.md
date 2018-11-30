---
title: Erstellen von windows10PFXImportCertificateProfile
description: Erstellen eines neuen windows10PFXImportCertificateProfile-Objekts.
ms.openlocfilehash: d1de09ebf79382cf1a656eaf3890e9139ebac2e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061140"
---
# <a name="create-windows10pfximportcertificateprofile"></a><span data-ttu-id="2c46a-103">Erstellen von windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2c46a-103">Create windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="2c46a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2c46a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c46a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2c46a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c46a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2c46a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c46a-107">Erstellen eines neuen [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c46a-107">Create a new [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2c46a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2c46a-108">Prerequisites</span></span>
<span data-ttu-id="2c46a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c46a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c46a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2c46a-111">Permission type</span></span>|<span data-ttu-id="2c46a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2c46a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c46a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2c46a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c46a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c46a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c46a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2c46a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c46a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c46a-116">Not supported.</span></span>|
|<span data-ttu-id="2c46a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2c46a-117">Application</span></span>|<span data-ttu-id="2c46a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c46a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c46a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c46a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2c46a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2c46a-120">Request headers</span></span>
|<span data-ttu-id="2c46a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2c46a-121">Header</span></span>|<span data-ttu-id="2c46a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2c46a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c46a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c46a-123">Authorization</span></span>|<span data-ttu-id="2c46a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2c46a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c46a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c46a-125">Accept</span></span>|<span data-ttu-id="2c46a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c46a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c46a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2c46a-127">Request body</span></span>
<span data-ttu-id="2c46a-128">Geben Sie im Textkörper Anforderung für das Objekt windows10PFXImportCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2c46a-128">In the request body, supply a JSON representation for the windows10PFXImportCertificateProfile object.</span></span>

<span data-ttu-id="2c46a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows10PFXImportCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="2c46a-129">The following table shows the properties that are required when you create the windows10PFXImportCertificateProfile.</span></span>

|<span data-ttu-id="2c46a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c46a-130">Property</span></span>|<span data-ttu-id="2c46a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2c46a-131">Type</span></span>|<span data-ttu-id="2c46a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c46a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c46a-133">id</span><span class="sxs-lookup"><span data-stu-id="2c46a-133">id</span></span>|<span data-ttu-id="2c46a-134">String</span><span class="sxs-lookup"><span data-stu-id="2c46a-134">String</span></span>|<span data-ttu-id="2c46a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2c46a-135">Key of the entity.</span></span> <span data-ttu-id="2c46a-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c46a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c46a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c46a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2c46a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c46a-138">DateTimeOffset</span></span>|<span data-ttu-id="2c46a-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c46a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2c46a-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c46a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c46a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c46a-141">roleScopeTagIds</span></span>|<span data-ttu-id="2c46a-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="2c46a-142">String collection</span></span>|<span data-ttu-id="2c46a-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="2c46a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2c46a-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c46a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c46a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2c46a-145">supportsScopeTags</span></span>|<span data-ttu-id="2c46a-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2c46a-146">Boolean</span></span>|<span data-ttu-id="2c46a-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2c46a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2c46a-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="2c46a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2c46a-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="2c46a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2c46a-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2c46a-150">This property is read-only.</span></span> <span data-ttu-id="2c46a-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c46a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c46a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c46a-152">createdDateTime</span></span>|<span data-ttu-id="2c46a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c46a-153">DateTimeOffset</span></span>|<span data-ttu-id="2c46a-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c46a-154">DateTime the object was created.</span></span> <span data-ttu-id="2c46a-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c46a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c46a-156">description</span><span class="sxs-lookup"><span data-stu-id="2c46a-156">description</span></span>|<span data-ttu-id="2c46a-157">String</span><span class="sxs-lookup"><span data-stu-id="2c46a-157">String</span></span>|<span data-ttu-id="2c46a-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2c46a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c46a-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c46a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c46a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2c46a-160">displayName</span></span>|<span data-ttu-id="2c46a-161">String</span><span class="sxs-lookup"><span data-stu-id="2c46a-161">String</span></span>|<span data-ttu-id="2c46a-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2c46a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c46a-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c46a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c46a-164">Version</span><span class="sxs-lookup"><span data-stu-id="2c46a-164">version</span></span>|<span data-ttu-id="2c46a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2c46a-165">Int32</span></span>|<span data-ttu-id="2c46a-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="2c46a-166">Version of the device configuration.</span></span> <span data-ttu-id="2c46a-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c46a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c46a-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="2c46a-168">keyStorageProvider</span></span>|[<span data-ttu-id="2c46a-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="2c46a-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="2c46a-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="2c46a-170">Not yet documented.</span></span> <span data-ttu-id="2c46a-171">Mögliche Werte sind: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="2c46a-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="2c46a-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c46a-172">Response</span></span>
<span data-ttu-id="2c46a-173">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2c46a-173">If successful, this method returns a `201 Created` response code and a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c46a-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2c46a-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="2c46a-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c46a-175">Request</span></span>
<span data-ttu-id="2c46a-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2c46a-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="2c46a-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c46a-177">Response</span></span>
<span data-ttu-id="2c46a-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2c46a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```





