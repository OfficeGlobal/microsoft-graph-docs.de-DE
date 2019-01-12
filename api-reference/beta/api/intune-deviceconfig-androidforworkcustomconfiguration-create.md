---
title: Erstellen von androidForWorkCustomConfiguration
description: Erstellen eines neuen AndroidForWorkCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04e7ad40814db2ec5064073930a5f6d5c6e599ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970136"
---
# <a name="create-androidforworkcustomconfiguration"></a><span data-ttu-id="78fcd-103">Erstellen von androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="78fcd-103">Create androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="78fcd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="78fcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78fcd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78fcd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78fcd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="78fcd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78fcd-107">Erstellen eines neuen [AndroidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="78fcd-107">Create a new [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78fcd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="78fcd-108">Prerequisites</span></span>
<span data-ttu-id="78fcd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78fcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78fcd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="78fcd-111">Permission type</span></span>|<span data-ttu-id="78fcd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="78fcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78fcd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="78fcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78fcd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78fcd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78fcd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="78fcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78fcd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78fcd-116">Not supported.</span></span>|
|<span data-ttu-id="78fcd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="78fcd-117">Application</span></span>|<span data-ttu-id="78fcd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78fcd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78fcd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="78fcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="78fcd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="78fcd-120">Request headers</span></span>
|<span data-ttu-id="78fcd-121">Header</span><span class="sxs-lookup"><span data-stu-id="78fcd-121">Header</span></span>|<span data-ttu-id="78fcd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="78fcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78fcd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78fcd-123">Authorization</span></span>|<span data-ttu-id="78fcd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="78fcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78fcd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="78fcd-125">Accept</span></span>|<span data-ttu-id="78fcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78fcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78fcd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="78fcd-127">Request body</span></span>
<span data-ttu-id="78fcd-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkCustomConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="78fcd-128">In the request body, supply a JSON representation for the androidForWorkCustomConfiguration object.</span></span>

<span data-ttu-id="78fcd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkCustomConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="78fcd-129">The following table shows the properties that are required when you create the androidForWorkCustomConfiguration.</span></span>

|<span data-ttu-id="78fcd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78fcd-130">Property</span></span>|<span data-ttu-id="78fcd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="78fcd-131">Type</span></span>|<span data-ttu-id="78fcd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78fcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78fcd-133">id</span><span class="sxs-lookup"><span data-stu-id="78fcd-133">id</span></span>|<span data-ttu-id="78fcd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78fcd-134">String</span></span>|<span data-ttu-id="78fcd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="78fcd-135">Key of the entity.</span></span> <span data-ttu-id="78fcd-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78fcd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78fcd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78fcd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="78fcd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78fcd-138">DateTimeOffset</span></span>|<span data-ttu-id="78fcd-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="78fcd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="78fcd-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78fcd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78fcd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="78fcd-141">roleScopeTagIds</span></span>|<span data-ttu-id="78fcd-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="78fcd-142">String collection</span></span>|<span data-ttu-id="78fcd-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="78fcd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="78fcd-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78fcd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78fcd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="78fcd-145">supportsScopeTags</span></span>|<span data-ttu-id="78fcd-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="78fcd-146">Boolean</span></span>|<span data-ttu-id="78fcd-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78fcd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="78fcd-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="78fcd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="78fcd-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="78fcd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="78fcd-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="78fcd-150">This property is read-only.</span></span> <span data-ttu-id="78fcd-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78fcd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78fcd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78fcd-152">createdDateTime</span></span>|<span data-ttu-id="78fcd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78fcd-153">DateTimeOffset</span></span>|<span data-ttu-id="78fcd-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="78fcd-154">DateTime the object was created.</span></span> <span data-ttu-id="78fcd-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78fcd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78fcd-156">description</span><span class="sxs-lookup"><span data-stu-id="78fcd-156">description</span></span>|<span data-ttu-id="78fcd-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78fcd-157">String</span></span>|<span data-ttu-id="78fcd-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="78fcd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="78fcd-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78fcd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78fcd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="78fcd-160">displayName</span></span>|<span data-ttu-id="78fcd-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78fcd-161">String</span></span>|<span data-ttu-id="78fcd-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="78fcd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="78fcd-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78fcd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78fcd-164">Version</span><span class="sxs-lookup"><span data-stu-id="78fcd-164">version</span></span>|<span data-ttu-id="78fcd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="78fcd-165">Int32</span></span>|<span data-ttu-id="78fcd-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="78fcd-166">Version of the device configuration.</span></span> <span data-ttu-id="78fcd-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="78fcd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78fcd-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="78fcd-168">omaSettings</span></span>|<span data-ttu-id="78fcd-169">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78fcd-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="78fcd-170">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="78fcd-170">OMA settings.</span></span> <span data-ttu-id="78fcd-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="78fcd-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="78fcd-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="78fcd-172">Response</span></span>
<span data-ttu-id="78fcd-173">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="78fcd-173">If successful, this method returns a `201 Created` response code and a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78fcd-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="78fcd-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="78fcd-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="78fcd-175">Request</span></span>
<span data-ttu-id="78fcd-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="78fcd-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="78fcd-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="78fcd-177">Response</span></span>
<span data-ttu-id="78fcd-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78fcd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





