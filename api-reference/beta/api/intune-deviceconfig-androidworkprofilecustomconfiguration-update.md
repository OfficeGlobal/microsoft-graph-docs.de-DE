---
title: AndroidWorkProfileCustomConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidWorkProfileCustomConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: a8a16a0e4fd9cb8e2f6970a63b723dae6fdebb25
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357820"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="dec72-103">AndroidWorkProfileCustomConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dec72-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="dec72-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dec72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dec72-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dec72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dec72-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dec72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dec72-107">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dec72-107">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dec72-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dec72-108">Prerequisites</span></span>
<span data-ttu-id="dec72-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dec72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dec72-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dec72-111">Permission type</span></span>|<span data-ttu-id="dec72-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dec72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dec72-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dec72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dec72-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dec72-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dec72-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dec72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dec72-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dec72-116">Not supported.</span></span>|
|<span data-ttu-id="dec72-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dec72-117">Application</span></span>|<span data-ttu-id="dec72-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dec72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dec72-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dec72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dec72-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dec72-120">Request headers</span></span>
|<span data-ttu-id="dec72-121">Header</span><span class="sxs-lookup"><span data-stu-id="dec72-121">Header</span></span>|<span data-ttu-id="dec72-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dec72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dec72-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="dec72-123">Authorization</span></span>|<span data-ttu-id="dec72-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dec72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dec72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dec72-125">Accept</span></span>|<span data-ttu-id="dec72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dec72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dec72-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dec72-127">Request body</span></span>
<span data-ttu-id="dec72-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="dec72-128">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="dec72-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="dec72-129">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="dec72-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dec72-130">Property</span></span>|<span data-ttu-id="dec72-131">Typ</span><span class="sxs-lookup"><span data-stu-id="dec72-131">Type</span></span>|<span data-ttu-id="dec72-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dec72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dec72-133">id</span><span class="sxs-lookup"><span data-stu-id="dec72-133">id</span></span>|<span data-ttu-id="dec72-134">String</span><span class="sxs-lookup"><span data-stu-id="dec72-134">String</span></span>|<span data-ttu-id="dec72-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dec72-135">Key of the entity.</span></span> <span data-ttu-id="dec72-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dec72-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dec72-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dec72-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dec72-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dec72-138">DateTimeOffset</span></span>|<span data-ttu-id="dec72-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="dec72-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dec72-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dec72-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dec72-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dec72-141">roleScopeTagIds</span></span>|<span data-ttu-id="dec72-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="dec72-142">String collection</span></span>|<span data-ttu-id="dec72-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="dec72-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dec72-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dec72-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dec72-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dec72-145">supportsScopeTags</span></span>|<span data-ttu-id="dec72-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="dec72-146">Boolean</span></span>|<span data-ttu-id="dec72-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dec72-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dec72-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="dec72-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dec72-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="dec72-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dec72-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dec72-150">This property is read-only.</span></span> <span data-ttu-id="dec72-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dec72-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dec72-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dec72-152">createdDateTime</span></span>|<span data-ttu-id="dec72-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dec72-153">DateTimeOffset</span></span>|<span data-ttu-id="dec72-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="dec72-154">DateTime the object was created.</span></span> <span data-ttu-id="dec72-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dec72-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dec72-156">description</span><span class="sxs-lookup"><span data-stu-id="dec72-156">description</span></span>|<span data-ttu-id="dec72-157">String</span><span class="sxs-lookup"><span data-stu-id="dec72-157">String</span></span>|<span data-ttu-id="dec72-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="dec72-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dec72-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dec72-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dec72-160">displayName</span><span class="sxs-lookup"><span data-stu-id="dec72-160">displayName</span></span>|<span data-ttu-id="dec72-161">String</span><span class="sxs-lookup"><span data-stu-id="dec72-161">String</span></span>|<span data-ttu-id="dec72-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="dec72-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dec72-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dec72-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dec72-164">Version</span><span class="sxs-lookup"><span data-stu-id="dec72-164">version</span></span>|<span data-ttu-id="dec72-165">Int32</span><span class="sxs-lookup"><span data-stu-id="dec72-165">Int32</span></span>|<span data-ttu-id="dec72-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="dec72-166">Version of the device configuration.</span></span> <span data-ttu-id="dec72-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dec72-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dec72-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="dec72-168">omaSettings</span></span>|<span data-ttu-id="dec72-169">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dec72-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="dec72-170">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="dec72-170">OMA settings.</span></span> <span data-ttu-id="dec72-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="dec72-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="dec72-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="dec72-172">Response</span></span>
<span data-ttu-id="dec72-173">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dec72-173">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dec72-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dec72-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="dec72-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dec72-175">Request</span></span>
<span data-ttu-id="dec72-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dec72-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dec72-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="dec72-177">Response</span></span>
<span data-ttu-id="dec72-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dec72-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





