---
title: AndroidForWorkCustomConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53238ad41d4f6ac91e3018cd3da831c6a2ec8ea3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807938"
---
# <a name="update-androidforworkcustomconfiguration"></a><span data-ttu-id="b415a-103">AndroidForWorkCustomConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b415a-103">Update androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="b415a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b415a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b415a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b415a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b415a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b415a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b415a-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b415a-107">Update the properties of a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b415a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b415a-108">Prerequisites</span></span>
<span data-ttu-id="b415a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b415a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b415a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b415a-111">Permission type</span></span>|<span data-ttu-id="b415a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b415a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b415a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b415a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b415a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b415a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b415a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b415a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b415a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b415a-116">Not supported.</span></span>|
|<span data-ttu-id="b415a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b415a-117">Application</span></span>|<span data-ttu-id="b415a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b415a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b415a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b415a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b415a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b415a-120">Request headers</span></span>
|<span data-ttu-id="b415a-121">Header</span><span class="sxs-lookup"><span data-stu-id="b415a-121">Header</span></span>|<span data-ttu-id="b415a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b415a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b415a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b415a-123">Authorization</span></span>|<span data-ttu-id="b415a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b415a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b415a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b415a-125">Accept</span></span>|<span data-ttu-id="b415a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b415a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b415a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b415a-127">Request body</span></span>
<span data-ttu-id="b415a-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b415a-128">In the request body, supply a JSON representation for the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

<span data-ttu-id="b415a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b415a-129">The following table shows the properties that are required when you create the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span></span>

|<span data-ttu-id="b415a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b415a-130">Property</span></span>|<span data-ttu-id="b415a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b415a-131">Type</span></span>|<span data-ttu-id="b415a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b415a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b415a-133">id</span><span class="sxs-lookup"><span data-stu-id="b415a-133">id</span></span>|<span data-ttu-id="b415a-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b415a-134">String</span></span>|<span data-ttu-id="b415a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b415a-135">Key of the entity.</span></span> <span data-ttu-id="b415a-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b415a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b415a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b415a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b415a-138">DateTimeOffset</span></span>|<span data-ttu-id="b415a-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b415a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b415a-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b415a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b415a-141">roleScopeTagIds</span></span>|<span data-ttu-id="b415a-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b415a-142">String collection</span></span>|<span data-ttu-id="b415a-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b415a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b415a-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b415a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b415a-145">supportsScopeTags</span></span>|<span data-ttu-id="b415a-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b415a-146">Boolean</span></span>|<span data-ttu-id="b415a-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b415a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b415a-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b415a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b415a-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b415a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b415a-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b415a-150">This property is read-only.</span></span> <span data-ttu-id="b415a-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b415a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b415a-152">createdDateTime</span></span>|<span data-ttu-id="b415a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b415a-153">DateTimeOffset</span></span>|<span data-ttu-id="b415a-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b415a-154">DateTime the object was created.</span></span> <span data-ttu-id="b415a-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b415a-156">description</span><span class="sxs-lookup"><span data-stu-id="b415a-156">description</span></span>|<span data-ttu-id="b415a-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b415a-157">String</span></span>|<span data-ttu-id="b415a-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b415a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b415a-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b415a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b415a-160">displayName</span></span>|<span data-ttu-id="b415a-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b415a-161">String</span></span>|<span data-ttu-id="b415a-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b415a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b415a-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b415a-164">Version</span><span class="sxs-lookup"><span data-stu-id="b415a-164">version</span></span>|<span data-ttu-id="b415a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b415a-165">Int32</span></span>|<span data-ttu-id="b415a-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b415a-166">Version of the device configuration.</span></span> <span data-ttu-id="b415a-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b415a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b415a-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="b415a-168">omaSettings</span></span>|<span data-ttu-id="b415a-169">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b415a-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="b415a-170">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="b415a-170">OMA settings.</span></span> <span data-ttu-id="b415a-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b415a-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b415a-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="b415a-172">Response</span></span>
<span data-ttu-id="b415a-173">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b415a-173">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b415a-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b415a-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="b415a-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b415a-175">Request</span></span>
<span data-ttu-id="b415a-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b415a-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 493

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="b415a-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="b415a-177">Response</span></span>
<span data-ttu-id="b415a-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b415a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
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





