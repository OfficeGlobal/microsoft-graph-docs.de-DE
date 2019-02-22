---
title: iosMobileAppConfiguration erstellen
description: Erstellen eines neuen iosMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fd62d2403272adbd95105ad87ba589d972f4870
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148097"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="52f88-103">iosMobileAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="52f88-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="52f88-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="52f88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52f88-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="52f88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52f88-106">Erstellen eines neuen [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="52f88-106">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52f88-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="52f88-107">Prerequisites</span></span>
<span data-ttu-id="52f88-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="52f88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="52f88-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52f88-110">Permission type</span></span>|<span data-ttu-id="52f88-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52f88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52f88-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52f88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52f88-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52f88-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52f88-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52f88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52f88-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52f88-115">Not supported.</span></span>|
|<span data-ttu-id="52f88-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52f88-116">Application</span></span>|<span data-ttu-id="52f88-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52f88-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52f88-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52f88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="52f88-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52f88-119">Request headers</span></span>
|<span data-ttu-id="52f88-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="52f88-120">Header</span></span>|<span data-ttu-id="52f88-121">Wert</span><span class="sxs-lookup"><span data-stu-id="52f88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52f88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52f88-122">Authorization</span></span>|<span data-ttu-id="52f88-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="52f88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52f88-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="52f88-124">Accept</span></span>|<span data-ttu-id="52f88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52f88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52f88-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52f88-126">Request body</span></span>
<span data-ttu-id="52f88-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs iosMobileAppConfiguration an.</span><span class="sxs-lookup"><span data-stu-id="52f88-127">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="52f88-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosMobileAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="52f88-128">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="52f88-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52f88-129">Property</span></span>|<span data-ttu-id="52f88-130">Typ</span><span class="sxs-lookup"><span data-stu-id="52f88-130">Type</span></span>|<span data-ttu-id="52f88-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52f88-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52f88-132">id</span><span class="sxs-lookup"><span data-stu-id="52f88-132">id</span></span>|<span data-ttu-id="52f88-133">string</span><span class="sxs-lookup"><span data-stu-id="52f88-133">String</span></span>|<span data-ttu-id="52f88-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="52f88-134">Key of the entity.</span></span> <span data-ttu-id="52f88-135">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52f88-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="52f88-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="52f88-136">targetedMobileApps</span></span>|<span data-ttu-id="52f88-137">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="52f88-137">String collection</span></span>|<span data-ttu-id="52f88-138">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="52f88-138">the associated app.</span></span> <span data-ttu-id="52f88-139">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52f88-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="52f88-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="52f88-140">roleScopeTagIds</span></span>|<span data-ttu-id="52f88-141">String collection</span><span class="sxs-lookup"><span data-stu-id="52f88-141">String collection</span></span>|<span data-ttu-id="52f88-142">Liste der Bereichs Tags für diese APP-Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="52f88-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="52f88-143">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52f88-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="52f88-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52f88-144">createdDateTime</span></span>|<span data-ttu-id="52f88-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52f88-145">DateTimeOffset</span></span>|<span data-ttu-id="52f88-146">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="52f88-146">DateTime the object was created.</span></span> <span data-ttu-id="52f88-147">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52f88-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="52f88-148">description</span><span class="sxs-lookup"><span data-stu-id="52f88-148">description</span></span>|<span data-ttu-id="52f88-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52f88-149">String</span></span>|<span data-ttu-id="52f88-150">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="52f88-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="52f88-151">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52f88-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="52f88-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52f88-152">lastModifiedDateTime</span></span>|<span data-ttu-id="52f88-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52f88-153">DateTimeOffset</span></span>|<span data-ttu-id="52f88-154">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="52f88-154">DateTime the object was last modified.</span></span> <span data-ttu-id="52f88-155">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52f88-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="52f88-156">displayName</span><span class="sxs-lookup"><span data-stu-id="52f88-156">displayName</span></span>|<span data-ttu-id="52f88-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52f88-157">String</span></span>|<span data-ttu-id="52f88-158">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="52f88-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="52f88-159">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52f88-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="52f88-160">version</span><span class="sxs-lookup"><span data-stu-id="52f88-160">version</span></span>|<span data-ttu-id="52f88-161">Int32</span><span class="sxs-lookup"><span data-stu-id="52f88-161">Int32</span></span>|<span data-ttu-id="52f88-162">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="52f88-162">Version of the device configuration.</span></span> <span data-ttu-id="52f88-163">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52f88-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="52f88-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="52f88-164">encodedSettingXml</span></span>|<span data-ttu-id="52f88-165">Binary</span><span class="sxs-lookup"><span data-stu-id="52f88-165">Binary</span></span>|<span data-ttu-id="52f88-166">Base64-binärcodierte MDM-App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="52f88-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="52f88-167">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="52f88-167">settings</span></span>|<span data-ttu-id="52f88-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="52f88-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="52f88-169">App-Konfigurationseinstellungselemente</span><span class="sxs-lookup"><span data-stu-id="52f88-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="52f88-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="52f88-170">Response</span></span>
<span data-ttu-id="52f88-171">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="52f88-171">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52f88-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52f88-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="52f88-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52f88-173">Request</span></span>
<span data-ttu-id="52f88-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52f88-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 596

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="52f88-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="52f88-175">Response</span></span>
<span data-ttu-id="52f88-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52f88-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 768

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```




