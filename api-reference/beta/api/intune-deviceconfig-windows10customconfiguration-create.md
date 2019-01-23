---
title: Erstellen von „windows10CustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows10CustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74bcada139f03995e4b86b15e7d5b41e43b15524
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393816"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="232a9-103">Erstellen von „windows10CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="232a9-103">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="232a9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="232a9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="232a9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="232a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="232a9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="232a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="232a9-107">Diese Methode erstellt ein neues Objekt des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-107">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="232a9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="232a9-108">Prerequisites</span></span>
<span data-ttu-id="232a9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="232a9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="232a9-111">Permission type</span></span>|<span data-ttu-id="232a9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="232a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="232a9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="232a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="232a9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="232a9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="232a9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="232a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="232a9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="232a9-116">Not supported.</span></span>|
|<span data-ttu-id="232a9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="232a9-117">Application</span></span>|<span data-ttu-id="232a9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="232a9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="232a9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="232a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="232a9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="232a9-120">Request headers</span></span>
|<span data-ttu-id="232a9-121">Header</span><span class="sxs-lookup"><span data-stu-id="232a9-121">Header</span></span>|<span data-ttu-id="232a9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="232a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="232a9-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="232a9-123">Authorization</span></span>|<span data-ttu-id="232a9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="232a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="232a9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="232a9-125">Accept</span></span>|<span data-ttu-id="232a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="232a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="232a9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="232a9-127">Request body</span></span>
<span data-ttu-id="232a9-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10CustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="232a9-128">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="232a9-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10CustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="232a9-129">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="232a9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="232a9-130">Property</span></span>|<span data-ttu-id="232a9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="232a9-131">Type</span></span>|<span data-ttu-id="232a9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="232a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="232a9-133">id</span><span class="sxs-lookup"><span data-stu-id="232a9-133">id</span></span>|<span data-ttu-id="232a9-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="232a9-134">String</span></span>|<span data-ttu-id="232a9-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="232a9-135">Key of the entity.</span></span> <span data-ttu-id="232a9-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="232a9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="232a9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="232a9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="232a9-138">DateTimeOffset</span></span>|<span data-ttu-id="232a9-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="232a9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="232a9-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="232a9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="232a9-141">roleScopeTagIds</span></span>|<span data-ttu-id="232a9-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="232a9-142">String collection</span></span>|<span data-ttu-id="232a9-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="232a9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="232a9-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="232a9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="232a9-145">supportsScopeTags</span></span>|<span data-ttu-id="232a9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="232a9-146">Boolean</span></span>|<span data-ttu-id="232a9-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="232a9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="232a9-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="232a9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="232a9-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="232a9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="232a9-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="232a9-150">This property is read-only.</span></span> <span data-ttu-id="232a9-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="232a9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="232a9-152">createdDateTime</span></span>|<span data-ttu-id="232a9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="232a9-153">DateTimeOffset</span></span>|<span data-ttu-id="232a9-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="232a9-154">DateTime the object was created.</span></span> <span data-ttu-id="232a9-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="232a9-156">description</span><span class="sxs-lookup"><span data-stu-id="232a9-156">description</span></span>|<span data-ttu-id="232a9-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="232a9-157">String</span></span>|<span data-ttu-id="232a9-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="232a9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="232a9-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="232a9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="232a9-160">displayName</span></span>|<span data-ttu-id="232a9-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="232a9-161">String</span></span>|<span data-ttu-id="232a9-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="232a9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="232a9-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="232a9-164">Version</span><span class="sxs-lookup"><span data-stu-id="232a9-164">version</span></span>|<span data-ttu-id="232a9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="232a9-165">Int32</span></span>|<span data-ttu-id="232a9-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="232a9-166">Version of the device configuration.</span></span> <span data-ttu-id="232a9-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="232a9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="232a9-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="232a9-168">omaSettings</span></span>|<span data-ttu-id="232a9-169">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="232a9-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="232a9-170">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="232a9-170">OMA settings.</span></span> <span data-ttu-id="232a9-171">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="232a9-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="232a9-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="232a9-172">Response</span></span>
<span data-ttu-id="232a9-173">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="232a9-173">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="232a9-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="232a9-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="232a9-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="232a9-175">Request</span></span>
<span data-ttu-id="232a9-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="232a9-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="232a9-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="232a9-177">Response</span></span>
<span data-ttu-id="232a9-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="232a9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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




