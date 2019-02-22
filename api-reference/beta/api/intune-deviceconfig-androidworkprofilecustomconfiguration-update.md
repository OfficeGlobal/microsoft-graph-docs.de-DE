---
title: AndroidWorkProfileCustomConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87d070e0edb73dc282f230361487199a50c9ebc8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149630"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="d7c20-103">AndroidWorkProfileCustomConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d7c20-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="d7c20-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7c20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7c20-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d7c20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7c20-106">Aktualisieren der Eigenschaften eines [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7c20-106">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7c20-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d7c20-107">Prerequisites</span></span>
<span data-ttu-id="d7c20-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d7c20-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7c20-110">Permission type</span></span>|<span data-ttu-id="d7c20-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7c20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7c20-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7c20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7c20-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c20-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7c20-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7c20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7c20-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7c20-115">Not supported.</span></span>|
|<span data-ttu-id="d7c20-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7c20-116">Application</span></span>|<span data-ttu-id="d7c20-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7c20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7c20-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7c20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d7c20-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7c20-119">Request headers</span></span>
|<span data-ttu-id="d7c20-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d7c20-120">Header</span></span>|<span data-ttu-id="d7c20-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d7c20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7c20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7c20-122">Authorization</span></span>|<span data-ttu-id="d7c20-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d7c20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7c20-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d7c20-124">Accept</span></span>|<span data-ttu-id="d7c20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7c20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7c20-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7c20-126">Request body</span></span>
<span data-ttu-id="d7c20-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d7c20-127">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="d7c20-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d7c20-128">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="d7c20-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7c20-129">Property</span></span>|<span data-ttu-id="d7c20-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d7c20-130">Type</span></span>|<span data-ttu-id="d7c20-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7c20-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7c20-132">id</span><span class="sxs-lookup"><span data-stu-id="d7c20-132">id</span></span>|<span data-ttu-id="d7c20-133">string</span><span class="sxs-lookup"><span data-stu-id="d7c20-133">String</span></span>|<span data-ttu-id="d7c20-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d7c20-134">Key of the entity.</span></span> <span data-ttu-id="d7c20-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7c20-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7c20-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d7c20-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7c20-137">DateTimeOffset</span></span>|<span data-ttu-id="d7c20-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7c20-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d7c20-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7c20-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="d7c20-140">roleScopeTagIds</span></span>|<span data-ttu-id="d7c20-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d7c20-141">String collection</span></span>|<span data-ttu-id="d7c20-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="d7c20-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d7c20-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7c20-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d7c20-144">supportsScopeTags</span></span>|<span data-ttu-id="d7c20-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d7c20-145">Boolean</span></span>|<span data-ttu-id="d7c20-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7c20-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d7c20-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="d7c20-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d7c20-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d7c20-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d7c20-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d7c20-149">This property is read-only.</span></span> <span data-ttu-id="d7c20-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7c20-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7c20-151">createdDateTime</span></span>|<span data-ttu-id="d7c20-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7c20-152">DateTimeOffset</span></span>|<span data-ttu-id="d7c20-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7c20-153">DateTime the object was created.</span></span> <span data-ttu-id="d7c20-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7c20-155">description</span><span class="sxs-lookup"><span data-stu-id="d7c20-155">description</span></span>|<span data-ttu-id="d7c20-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7c20-156">String</span></span>|<span data-ttu-id="d7c20-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d7c20-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d7c20-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7c20-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d7c20-159">displayName</span></span>|<span data-ttu-id="d7c20-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7c20-160">String</span></span>|<span data-ttu-id="d7c20-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d7c20-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d7c20-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7c20-163">Version</span><span class="sxs-lookup"><span data-stu-id="d7c20-163">version</span></span>|<span data-ttu-id="d7c20-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c20-164">Int32</span></span>|<span data-ttu-id="d7c20-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d7c20-165">Version of the device configuration.</span></span> <span data-ttu-id="d7c20-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c20-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7c20-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="d7c20-167">omaSettings</span></span>|<span data-ttu-id="d7c20-168">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7c20-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="d7c20-169">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="d7c20-169">OMA settings.</span></span> <span data-ttu-id="d7c20-170">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d7c20-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d7c20-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7c20-171">Response</span></span>
<span data-ttu-id="d7c20-172">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d7c20-172">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7c20-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7c20-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7c20-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7c20-174">Request</span></span>
<span data-ttu-id="d7c20-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7c20-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d7c20-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7c20-176">Response</span></span>
<span data-ttu-id="d7c20-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7c20-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




