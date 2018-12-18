---
title: IosEducationDeviceConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosEducationDeviceConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: c934fa3c6274ca6b0149958cde9e2e231c2236f1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325123"
---
# <a name="update-ioseducationdeviceconfiguration"></a><span data-ttu-id="2edf9-103">IosEducationDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2edf9-103">Update iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="2edf9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2edf9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2edf9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2edf9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2edf9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2edf9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2edf9-107">Aktualisieren Sie die Eigenschaften eines [IosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2edf9-107">Update the properties of a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2edf9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2edf9-108">Prerequisites</span></span>
<span data-ttu-id="2edf9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2edf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2edf9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2edf9-111">Permission type</span></span>|<span data-ttu-id="2edf9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2edf9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2edf9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2edf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2edf9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2edf9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2edf9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2edf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2edf9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2edf9-116">Not supported.</span></span>|
|<span data-ttu-id="2edf9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2edf9-117">Application</span></span>|<span data-ttu-id="2edf9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2edf9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2edf9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2edf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2edf9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2edf9-120">Request headers</span></span>
|<span data-ttu-id="2edf9-121">Header</span><span class="sxs-lookup"><span data-stu-id="2edf9-121">Header</span></span>|<span data-ttu-id="2edf9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2edf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2edf9-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2edf9-123">Authorization</span></span>|<span data-ttu-id="2edf9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2edf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2edf9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2edf9-125">Accept</span></span>|<span data-ttu-id="2edf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2edf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2edf9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2edf9-127">Request body</span></span>
<span data-ttu-id="2edf9-128">Geben Sie im Textkörper Anforderung für das Objekt [IosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2edf9-128">In the request body, supply a JSON representation for the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

<span data-ttu-id="2edf9-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="2edf9-129">The following table shows the properties that are required when you create the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span></span>

|<span data-ttu-id="2edf9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2edf9-130">Property</span></span>|<span data-ttu-id="2edf9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2edf9-131">Type</span></span>|<span data-ttu-id="2edf9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2edf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2edf9-133">id</span><span class="sxs-lookup"><span data-stu-id="2edf9-133">id</span></span>|<span data-ttu-id="2edf9-134">String</span><span class="sxs-lookup"><span data-stu-id="2edf9-134">String</span></span>|<span data-ttu-id="2edf9-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2edf9-135">Key of the entity.</span></span> <span data-ttu-id="2edf9-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2edf9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2edf9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2edf9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2edf9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2edf9-138">DateTimeOffset</span></span>|<span data-ttu-id="2edf9-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2edf9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2edf9-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2edf9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2edf9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2edf9-141">roleScopeTagIds</span></span>|<span data-ttu-id="2edf9-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="2edf9-142">String collection</span></span>|<span data-ttu-id="2edf9-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="2edf9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2edf9-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2edf9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2edf9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2edf9-145">supportsScopeTags</span></span>|<span data-ttu-id="2edf9-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2edf9-146">Boolean</span></span>|<span data-ttu-id="2edf9-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2edf9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2edf9-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="2edf9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2edf9-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="2edf9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2edf9-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2edf9-150">This property is read-only.</span></span> <span data-ttu-id="2edf9-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2edf9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2edf9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2edf9-152">createdDateTime</span></span>|<span data-ttu-id="2edf9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2edf9-153">DateTimeOffset</span></span>|<span data-ttu-id="2edf9-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2edf9-154">DateTime the object was created.</span></span> <span data-ttu-id="2edf9-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2edf9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2edf9-156">description</span><span class="sxs-lookup"><span data-stu-id="2edf9-156">description</span></span>|<span data-ttu-id="2edf9-157">String</span><span class="sxs-lookup"><span data-stu-id="2edf9-157">String</span></span>|<span data-ttu-id="2edf9-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2edf9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2edf9-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2edf9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2edf9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2edf9-160">displayName</span></span>|<span data-ttu-id="2edf9-161">String</span><span class="sxs-lookup"><span data-stu-id="2edf9-161">String</span></span>|<span data-ttu-id="2edf9-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2edf9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2edf9-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2edf9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2edf9-164">Version</span><span class="sxs-lookup"><span data-stu-id="2edf9-164">version</span></span>|<span data-ttu-id="2edf9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2edf9-165">Int32</span></span>|<span data-ttu-id="2edf9-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="2edf9-166">Version of the device configuration.</span></span> <span data-ttu-id="2edf9-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2edf9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2edf9-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="2edf9-168">Response</span></span>
<span data-ttu-id="2edf9-169">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2edf9-169">If successful, this method returns a `200 OK` response code and an updated [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2edf9-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2edf9-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="2edf9-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2edf9-171">Request</span></span>
<span data-ttu-id="2edf9-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2edf9-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 255

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="2edf9-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="2edf9-173">Response</span></span>
<span data-ttu-id="2edf9-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2edf9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```





