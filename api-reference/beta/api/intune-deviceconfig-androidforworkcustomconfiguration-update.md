---
title: AndroidForWorkCustomConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidForWorkCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7b0fe0f410cfa6b4873609896d85e72857f31e6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963688"
---
# <a name="update-androidforworkcustomconfiguration"></a><span data-ttu-id="ba109-103">AndroidForWorkCustomConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ba109-103">Update androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="ba109-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba109-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba109-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ba109-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba109-106">Aktualisieren der Eigenschaften eines [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ba109-106">Update the properties of a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba109-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ba109-107">Prerequisites</span></span>
<span data-ttu-id="ba109-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba109-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba109-110">Permission type</span></span>|<span data-ttu-id="ba109-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba109-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba109-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba109-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba109-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba109-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba109-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba109-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba109-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba109-115">Not supported.</span></span>|
|<span data-ttu-id="ba109-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba109-116">Application</span></span>|<span data-ttu-id="ba109-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba109-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba109-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba109-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ba109-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba109-119">Request headers</span></span>
|<span data-ttu-id="ba109-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ba109-120">Header</span></span>|<span data-ttu-id="ba109-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ba109-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba109-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba109-122">Authorization</span></span>|<span data-ttu-id="ba109-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ba109-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba109-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ba109-124">Accept</span></span>|<span data-ttu-id="ba109-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba109-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba109-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba109-126">Request body</span></span>
<span data-ttu-id="ba109-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ba109-127">In the request body, supply a JSON representation for the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

<span data-ttu-id="ba109-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ba109-128">The following table shows the properties that are required when you create the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span></span>

|<span data-ttu-id="ba109-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba109-129">Property</span></span>|<span data-ttu-id="ba109-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ba109-130">Type</span></span>|<span data-ttu-id="ba109-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba109-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba109-132">id</span><span class="sxs-lookup"><span data-stu-id="ba109-132">id</span></span>|<span data-ttu-id="ba109-133">String</span><span class="sxs-lookup"><span data-stu-id="ba109-133">String</span></span>|<span data-ttu-id="ba109-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ba109-134">Key of the entity.</span></span> <span data-ttu-id="ba109-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba109-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba109-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba109-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ba109-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba109-137">DateTimeOffset</span></span>|<span data-ttu-id="ba109-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ba109-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ba109-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba109-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba109-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ba109-140">roleScopeTagIds</span></span>|<span data-ttu-id="ba109-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ba109-141">String collection</span></span>|<span data-ttu-id="ba109-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="ba109-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ba109-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba109-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba109-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ba109-144">supportsScopeTags</span></span>|<span data-ttu-id="ba109-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba109-145">Boolean</span></span>|<span data-ttu-id="ba109-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba109-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ba109-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="ba109-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ba109-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ba109-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ba109-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ba109-149">This property is read-only.</span></span> <span data-ttu-id="ba109-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba109-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba109-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba109-151">createdDateTime</span></span>|<span data-ttu-id="ba109-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba109-152">DateTimeOffset</span></span>|<span data-ttu-id="ba109-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ba109-153">DateTime the object was created.</span></span> <span data-ttu-id="ba109-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba109-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba109-155">description</span><span class="sxs-lookup"><span data-stu-id="ba109-155">description</span></span>|<span data-ttu-id="ba109-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba109-156">String</span></span>|<span data-ttu-id="ba109-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ba109-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ba109-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba109-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba109-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ba109-159">displayName</span></span>|<span data-ttu-id="ba109-160">String</span><span class="sxs-lookup"><span data-stu-id="ba109-160">String</span></span>|<span data-ttu-id="ba109-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ba109-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ba109-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba109-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba109-163">Version</span><span class="sxs-lookup"><span data-stu-id="ba109-163">version</span></span>|<span data-ttu-id="ba109-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ba109-164">Int32</span></span>|<span data-ttu-id="ba109-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ba109-165">Version of the device configuration.</span></span> <span data-ttu-id="ba109-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba109-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba109-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ba109-167">omaSettings</span></span>|<span data-ttu-id="ba109-168">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba109-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ba109-169">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="ba109-169">OMA settings.</span></span> <span data-ttu-id="ba109-170">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ba109-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ba109-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba109-171">Response</span></span>
<span data-ttu-id="ba109-172">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ba109-172">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba109-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba109-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba109-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba109-174">Request</span></span>
<span data-ttu-id="ba109-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ba109-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="ba109-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba109-176">Response</span></span>
<span data-ttu-id="ba109-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ba109-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




