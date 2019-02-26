---
title: iosMobileAppConfiguration erstellen
description: Erstellen eines neuen iosMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e032d93a65b5827afdeffd498e745339b9d4e3a1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257946"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="8067e-103">iosMobileAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="8067e-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="8067e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8067e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8067e-105">Erstellen eines neuen [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8067e-105">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8067e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8067e-106">Prerequisites</span></span>
<span data-ttu-id="8067e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8067e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8067e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8067e-109">Permission type</span></span>|<span data-ttu-id="8067e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8067e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8067e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8067e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8067e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8067e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8067e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8067e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8067e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8067e-114">Not supported.</span></span>|
|<span data-ttu-id="8067e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8067e-115">Application</span></span>|<span data-ttu-id="8067e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8067e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8067e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8067e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8067e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8067e-118">Request headers</span></span>
|<span data-ttu-id="8067e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8067e-119">Header</span></span>|<span data-ttu-id="8067e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8067e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8067e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8067e-121">Authorization</span></span>|<span data-ttu-id="8067e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8067e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8067e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8067e-123">Accept</span></span>|<span data-ttu-id="8067e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8067e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8067e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8067e-125">Request body</span></span>
<span data-ttu-id="8067e-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs iosMobileAppConfiguration an.</span><span class="sxs-lookup"><span data-stu-id="8067e-126">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="8067e-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosMobileAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="8067e-127">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="8067e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8067e-128">Property</span></span>|<span data-ttu-id="8067e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8067e-129">Type</span></span>|<span data-ttu-id="8067e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8067e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8067e-131">id</span><span class="sxs-lookup"><span data-stu-id="8067e-131">id</span></span>|<span data-ttu-id="8067e-132">string</span><span class="sxs-lookup"><span data-stu-id="8067e-132">String</span></span>|<span data-ttu-id="8067e-133">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="8067e-133">Key of the entity.</span></span> <span data-ttu-id="8067e-134">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8067e-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8067e-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="8067e-135">targetedMobileApps</span></span>|<span data-ttu-id="8067e-136">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8067e-136">String collection</span></span>|<span data-ttu-id="8067e-137">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="8067e-137">the associated app.</span></span> <span data-ttu-id="8067e-138">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8067e-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8067e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8067e-139">createdDateTime</span></span>|<span data-ttu-id="8067e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8067e-140">DateTimeOffset</span></span>|<span data-ttu-id="8067e-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8067e-141">DateTime the object was created.</span></span> <span data-ttu-id="8067e-142">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8067e-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8067e-143">description</span><span class="sxs-lookup"><span data-stu-id="8067e-143">description</span></span>|<span data-ttu-id="8067e-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8067e-144">String</span></span>|<span data-ttu-id="8067e-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8067e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8067e-146">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8067e-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8067e-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8067e-147">lastModifiedDateTime</span></span>|<span data-ttu-id="8067e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8067e-148">DateTimeOffset</span></span>|<span data-ttu-id="8067e-149">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8067e-149">DateTime the object was last modified.</span></span> <span data-ttu-id="8067e-150">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8067e-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8067e-151">displayName</span><span class="sxs-lookup"><span data-stu-id="8067e-151">displayName</span></span>|<span data-ttu-id="8067e-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8067e-152">String</span></span>|<span data-ttu-id="8067e-153">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8067e-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8067e-154">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8067e-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8067e-155">version</span><span class="sxs-lookup"><span data-stu-id="8067e-155">version</span></span>|<span data-ttu-id="8067e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8067e-156">Int32</span></span>|<span data-ttu-id="8067e-157">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8067e-157">Version of the device configuration.</span></span> <span data-ttu-id="8067e-158">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8067e-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8067e-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="8067e-159">encodedSettingXml</span></span>|<span data-ttu-id="8067e-160">Binary</span><span class="sxs-lookup"><span data-stu-id="8067e-160">Binary</span></span>|<span data-ttu-id="8067e-161">Base64-binärcodierte MDM-App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="8067e-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="8067e-162">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="8067e-162">settings</span></span>|<span data-ttu-id="8067e-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8067e-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="8067e-164">App-Konfigurationseinstellungselemente</span><span class="sxs-lookup"><span data-stu-id="8067e-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="8067e-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="8067e-165">Response</span></span>
<span data-ttu-id="8067e-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8067e-166">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8067e-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8067e-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="8067e-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8067e-168">Request</span></span>
<span data-ttu-id="8067e-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8067e-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8067e-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="8067e-170">Response</span></span>
<span data-ttu-id="8067e-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8067e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



