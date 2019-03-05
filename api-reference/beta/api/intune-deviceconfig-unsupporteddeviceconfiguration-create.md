---
title: UnsupportedDeviceConfiguration erstellen
description: Erstellen eines neuen unsupportedDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8310d553382d754b386ced1bd7fbac7f6811cf8c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149546"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="6f8eb-103">UnsupportedDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="6f8eb-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="6f8eb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f8eb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f8eb-106">Erstellen eines neuen [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-106">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f8eb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f8eb-107">Prerequisites</span></span>
<span data-ttu-id="6f8eb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6f8eb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f8eb-110">Permission type</span></span>|<span data-ttu-id="6f8eb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f8eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f8eb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f8eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f8eb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f8eb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f8eb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f8eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f8eb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f8eb-115">Not supported.</span></span>|
|<span data-ttu-id="6f8eb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f8eb-116">Application</span></span>|<span data-ttu-id="6f8eb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f8eb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f8eb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f8eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6f8eb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f8eb-119">Request headers</span></span>
|<span data-ttu-id="6f8eb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6f8eb-120">Header</span></span>|<span data-ttu-id="6f8eb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6f8eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f8eb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f8eb-122">Authorization</span></span>|<span data-ttu-id="6f8eb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f8eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f8eb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6f8eb-124">Accept</span></span>|<span data-ttu-id="6f8eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f8eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f8eb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f8eb-126">Request body</span></span>
<span data-ttu-id="6f8eb-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das unsupportedDeviceConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-127">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="6f8eb-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der unsupportedDeviceConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-128">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="6f8eb-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f8eb-129">Property</span></span>|<span data-ttu-id="6f8eb-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6f8eb-130">Type</span></span>|<span data-ttu-id="6f8eb-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f8eb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f8eb-132">id</span><span class="sxs-lookup"><span data-stu-id="6f8eb-132">id</span></span>|<span data-ttu-id="6f8eb-133">string</span><span class="sxs-lookup"><span data-stu-id="6f8eb-133">String</span></span>|<span data-ttu-id="6f8eb-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6f8eb-134">Key of the entity.</span></span> <span data-ttu-id="6f8eb-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8eb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f8eb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6f8eb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f8eb-137">DateTimeOffset</span></span>|<span data-ttu-id="6f8eb-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6f8eb-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8eb-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="6f8eb-140">roleScopeTagIds</span></span>|<span data-ttu-id="6f8eb-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6f8eb-141">String collection</span></span>|<span data-ttu-id="6f8eb-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f8eb-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8eb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f8eb-144">supportsScopeTags</span></span>|<span data-ttu-id="6f8eb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f8eb-145">Boolean</span></span>|<span data-ttu-id="6f8eb-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f8eb-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f8eb-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f8eb-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-149">This property is read-only.</span></span> <span data-ttu-id="6f8eb-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8eb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f8eb-151">createdDateTime</span></span>|<span data-ttu-id="6f8eb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f8eb-152">DateTimeOffset</span></span>|<span data-ttu-id="6f8eb-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-153">DateTime the object was created.</span></span> <span data-ttu-id="6f8eb-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8eb-155">description</span><span class="sxs-lookup"><span data-stu-id="6f8eb-155">description</span></span>|<span data-ttu-id="6f8eb-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f8eb-156">String</span></span>|<span data-ttu-id="6f8eb-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f8eb-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8eb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6f8eb-159">displayName</span></span>|<span data-ttu-id="6f8eb-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f8eb-160">String</span></span>|<span data-ttu-id="6f8eb-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f8eb-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8eb-163">Version</span><span class="sxs-lookup"><span data-stu-id="6f8eb-163">version</span></span>|<span data-ttu-id="6f8eb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6f8eb-164">Int32</span></span>|<span data-ttu-id="6f8eb-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-165">Version of the device configuration.</span></span> <span data-ttu-id="6f8eb-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8eb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8eb-167">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="6f8eb-167">originalEntityTypeName</span></span>|<span data-ttu-id="6f8eb-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f8eb-168">String</span></span>|<span data-ttu-id="6f8eb-169">Der Typ der Entität, die andernfalls zurückgegeben würde.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-169">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="6f8eb-170">Details</span><span class="sxs-lookup"><span data-stu-id="6f8eb-170">details</span></span>|<span data-ttu-id="6f8eb-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f8eb-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="6f8eb-172">Details, die beschreiben, warum die Entität nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-172">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="6f8eb-173">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-173">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6f8eb-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f8eb-174">Response</span></span>
<span data-ttu-id="6f8eb-175">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-175">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f8eb-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f8eb-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f8eb-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f8eb-177">Request</span></span>
<span data-ttu-id="6f8eb-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6f8eb-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f8eb-179">Response</span></span>
<span data-ttu-id="6f8eb-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f8eb-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 690

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```




