---
title: iosMobileAppConfiguration erstellen
description: Erstellen eines neuen iosMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d85a55e8ea645b451f2248ab8d82836238b6c8e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822323"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="5a3a3-103">iosMobileAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="5a3a3-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="5a3a3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a3a3-105">Erstellen eines neuen [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-105">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a3a3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5a3a3-106">Prerequisites</span></span>
<span data-ttu-id="5a3a3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a3a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a3a3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a3a3-109">Permission type</span></span>|<span data-ttu-id="5a3a3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a3a3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a3a3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a3a3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5a3a3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a3a3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a3a3-114">Not supported.</span></span>|
|<span data-ttu-id="5a3a3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a3a3-115">Application</span></span>|<span data-ttu-id="5a3a3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a3a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a3a3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a3a3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5a3a3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a3a3-118">Request headers</span></span>
|<span data-ttu-id="5a3a3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5a3a3-119">Header</span></span>|<span data-ttu-id="5a3a3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5a3a3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a3a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a3a3-121">Authorization</span></span>|<span data-ttu-id="5a3a3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5a3a3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a3a3-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5a3a3-123">Accept</span></span>|<span data-ttu-id="5a3a3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a3a3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a3a3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a3a3-125">Request body</span></span>
<span data-ttu-id="5a3a3-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs iosMobileAppConfiguration an.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-126">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="5a3a3-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosMobileAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-127">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="5a3a3-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a3a3-128">Property</span></span>|<span data-ttu-id="5a3a3-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5a3a3-129">Type</span></span>|<span data-ttu-id="5a3a3-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a3a3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a3a3-131">id</span><span class="sxs-lookup"><span data-stu-id="5a3a3-131">id</span></span>|<span data-ttu-id="5a3a3-132">String</span><span class="sxs-lookup"><span data-stu-id="5a3a3-132">String</span></span>|<span data-ttu-id="5a3a3-133">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-133">Key of the entity.</span></span> <span data-ttu-id="5a3a3-134">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5a3a3-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="5a3a3-135">targetedMobileApps</span></span>|<span data-ttu-id="5a3a3-136">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5a3a3-136">String collection</span></span>|<span data-ttu-id="5a3a3-137">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-137">the associated app.</span></span> <span data-ttu-id="5a3a3-138">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5a3a3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a3a3-139">createdDateTime</span></span>|<span data-ttu-id="5a3a3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a3a3-140">DateTimeOffset</span></span>|<span data-ttu-id="5a3a3-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-141">DateTime the object was created.</span></span> <span data-ttu-id="5a3a3-142">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5a3a3-143">description</span><span class="sxs-lookup"><span data-stu-id="5a3a3-143">description</span></span>|<span data-ttu-id="5a3a3-144">String</span><span class="sxs-lookup"><span data-stu-id="5a3a3-144">String</span></span>|<span data-ttu-id="5a3a3-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5a3a3-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5a3a3-146">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5a3a3-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a3a3-147">lastModifiedDateTime</span></span>|<span data-ttu-id="5a3a3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a3a3-148">DateTimeOffset</span></span>|<span data-ttu-id="5a3a3-149">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-149">DateTime the object was last modified.</span></span> <span data-ttu-id="5a3a3-150">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5a3a3-151">displayName</span><span class="sxs-lookup"><span data-stu-id="5a3a3-151">displayName</span></span>|<span data-ttu-id="5a3a3-152">String</span><span class="sxs-lookup"><span data-stu-id="5a3a3-152">String</span></span>|<span data-ttu-id="5a3a3-153">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5a3a3-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5a3a3-154">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5a3a3-155">version</span><span class="sxs-lookup"><span data-stu-id="5a3a3-155">version</span></span>|<span data-ttu-id="5a3a3-156">Int32</span><span class="sxs-lookup"><span data-stu-id="5a3a3-156">Int32</span></span>|<span data-ttu-id="5a3a3-157">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-157">Version of the device configuration.</span></span> <span data-ttu-id="5a3a3-158">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a3a3-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5a3a3-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="5a3a3-159">encodedSettingXml</span></span>|<span data-ttu-id="5a3a3-160">Binary</span><span class="sxs-lookup"><span data-stu-id="5a3a3-160">Binary</span></span>|<span data-ttu-id="5a3a3-161">Base64-binärcodierte MDM-App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="5a3a3-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="5a3a3-162">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="5a3a3-162">settings</span></span>|<span data-ttu-id="5a3a3-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5a3a3-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="5a3a3-164">App-Konfigurationseinstellungselemente</span><span class="sxs-lookup"><span data-stu-id="5a3a3-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="5a3a3-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a3a3-165">Response</span></span>
<span data-ttu-id="5a3a3-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-166">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a3a3-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a3a3-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a3a3-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a3a3-168">Request</span></span>
<span data-ttu-id="5a3a3-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 534

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
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

### <a name="response"></a><span data-ttu-id="5a3a3-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a3a3-170">Response</span></span>
<span data-ttu-id="5a3a3-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a3a3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
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



