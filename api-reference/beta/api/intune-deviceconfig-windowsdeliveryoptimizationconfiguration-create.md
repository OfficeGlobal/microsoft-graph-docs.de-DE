---
title: Erstellen von windowsDeliveryOptimizationConfiguration
description: Erstellen eines neuen WindowsDeliveryOptimizationConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b469b93c81655ad3f071be1ffdbd36b18f32258
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430106"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="5425e-103">Erstellen von windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5425e-103">Create windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="5425e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5425e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5425e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5425e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5425e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5425e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5425e-107">Erstellen eines neuen [WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5425e-107">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5425e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5425e-108">Prerequisites</span></span>
<span data-ttu-id="5425e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5425e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5425e-111">Permission type</span></span>|<span data-ttu-id="5425e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5425e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5425e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5425e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5425e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5425e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5425e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5425e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5425e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5425e-116">Not supported.</span></span>|
|<span data-ttu-id="5425e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5425e-117">Application</span></span>|<span data-ttu-id="5425e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5425e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5425e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5425e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5425e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5425e-120">Request headers</span></span>
|<span data-ttu-id="5425e-121">Header</span><span class="sxs-lookup"><span data-stu-id="5425e-121">Header</span></span>|<span data-ttu-id="5425e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5425e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5425e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5425e-123">Authorization</span></span>|<span data-ttu-id="5425e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5425e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5425e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5425e-125">Accept</span></span>|<span data-ttu-id="5425e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5425e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5425e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5425e-127">Request body</span></span>
<span data-ttu-id="5425e-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsDeliveryOptimizationConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5425e-128">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="5425e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsDeliveryOptimizationConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="5425e-129">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="5425e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5425e-130">Property</span></span>|<span data-ttu-id="5425e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5425e-131">Type</span></span>|<span data-ttu-id="5425e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5425e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5425e-133">id</span><span class="sxs-lookup"><span data-stu-id="5425e-133">id</span></span>|<span data-ttu-id="5425e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5425e-134">String</span></span>|<span data-ttu-id="5425e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5425e-135">Key of the entity.</span></span> <span data-ttu-id="5425e-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5425e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5425e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5425e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5425e-138">DateTimeOffset</span></span>|<span data-ttu-id="5425e-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5425e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5425e-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5425e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5425e-141">roleScopeTagIds</span></span>|<span data-ttu-id="5425e-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="5425e-142">String collection</span></span>|<span data-ttu-id="5425e-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="5425e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5425e-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5425e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5425e-145">supportsScopeTags</span></span>|<span data-ttu-id="5425e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5425e-146">Boolean</span></span>|<span data-ttu-id="5425e-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5425e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5425e-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="5425e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5425e-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="5425e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5425e-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5425e-150">This property is read-only.</span></span> <span data-ttu-id="5425e-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5425e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5425e-152">createdDateTime</span></span>|<span data-ttu-id="5425e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5425e-153">DateTimeOffset</span></span>|<span data-ttu-id="5425e-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5425e-154">DateTime the object was created.</span></span> <span data-ttu-id="5425e-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5425e-156">description</span><span class="sxs-lookup"><span data-stu-id="5425e-156">description</span></span>|<span data-ttu-id="5425e-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5425e-157">String</span></span>|<span data-ttu-id="5425e-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5425e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5425e-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5425e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5425e-160">displayName</span></span>|<span data-ttu-id="5425e-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5425e-161">String</span></span>|<span data-ttu-id="5425e-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5425e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5425e-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5425e-164">Version</span><span class="sxs-lookup"><span data-stu-id="5425e-164">version</span></span>|<span data-ttu-id="5425e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5425e-165">Int32</span></span>|<span data-ttu-id="5425e-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5425e-166">Version of the device configuration.</span></span> <span data-ttu-id="5425e-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5425e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5425e-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="5425e-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="5425e-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="5425e-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="5425e-170">Gibt die Methode zum Herunterladen dieser Übermittlung Optimierung können Sie Netzwerkbandbreite für große Verteilung von Inhalten Szenarien verwalten.</span><span class="sxs-lookup"><span data-stu-id="5425e-170">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="5425e-171">Mögliche Werte sind: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="5425e-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|



## <a name="response"></a><span data-ttu-id="5425e-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="5425e-172">Response</span></span>
<span data-ttu-id="5425e-173">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5425e-173">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5425e-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5425e-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="5425e-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5425e-175">Request</span></span>
<span data-ttu-id="5425e-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5425e-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly"
}
```

### <a name="response"></a><span data-ttu-id="5425e-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="5425e-177">Response</span></span>
<span data-ttu-id="5425e-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5425e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly"
}
```



