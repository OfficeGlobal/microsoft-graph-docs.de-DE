---
title: IosMobileAppConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines iosMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 67aa52f71303914aaa7173f266e60ad29d9fa811
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979131"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="60a36-103">IosMobileAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="60a36-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="60a36-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="60a36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60a36-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60a36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60a36-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="60a36-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60a36-107">Aktualisieren der Eigenschaften eines [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="60a36-107">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60a36-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="60a36-108">Prerequisites</span></span>
<span data-ttu-id="60a36-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60a36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a36-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60a36-111">Permission type</span></span>|<span data-ttu-id="60a36-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60a36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60a36-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60a36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60a36-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60a36-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60a36-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60a36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60a36-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60a36-116">Not supported.</span></span>|
|<span data-ttu-id="60a36-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60a36-117">Application</span></span>|<span data-ttu-id="60a36-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60a36-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60a36-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60a36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="60a36-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60a36-120">Request headers</span></span>
|<span data-ttu-id="60a36-121">Header</span><span class="sxs-lookup"><span data-stu-id="60a36-121">Header</span></span>|<span data-ttu-id="60a36-122">Wert</span><span class="sxs-lookup"><span data-stu-id="60a36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60a36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a36-123">Authorization</span></span>|<span data-ttu-id="60a36-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="60a36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60a36-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="60a36-125">Accept</span></span>|<span data-ttu-id="60a36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60a36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60a36-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60a36-127">Request body</span></span>
<span data-ttu-id="60a36-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="60a36-128">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="60a36-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="60a36-129">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="60a36-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60a36-130">Property</span></span>|<span data-ttu-id="60a36-131">Typ</span><span class="sxs-lookup"><span data-stu-id="60a36-131">Type</span></span>|<span data-ttu-id="60a36-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60a36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60a36-133">id</span><span class="sxs-lookup"><span data-stu-id="60a36-133">id</span></span>|<span data-ttu-id="60a36-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60a36-134">String</span></span>|<span data-ttu-id="60a36-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="60a36-135">Key of the entity.</span></span> <span data-ttu-id="60a36-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60a36-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="60a36-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="60a36-137">targetedMobileApps</span></span>|<span data-ttu-id="60a36-138">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="60a36-138">String collection</span></span>|<span data-ttu-id="60a36-139">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="60a36-139">the associated app.</span></span> <span data-ttu-id="60a36-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60a36-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="60a36-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="60a36-141">roleScopeTagIds</span></span>|<span data-ttu-id="60a36-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="60a36-142">String collection</span></span>|<span data-ttu-id="60a36-143">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="60a36-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="60a36-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60a36-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="60a36-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60a36-145">createdDateTime</span></span>|<span data-ttu-id="60a36-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60a36-146">DateTimeOffset</span></span>|<span data-ttu-id="60a36-147">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="60a36-147">DateTime the object was created.</span></span> <span data-ttu-id="60a36-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60a36-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="60a36-149">description</span><span class="sxs-lookup"><span data-stu-id="60a36-149">description</span></span>|<span data-ttu-id="60a36-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60a36-150">String</span></span>|<span data-ttu-id="60a36-151">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="60a36-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="60a36-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60a36-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="60a36-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60a36-153">lastModifiedDateTime</span></span>|<span data-ttu-id="60a36-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60a36-154">DateTimeOffset</span></span>|<span data-ttu-id="60a36-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="60a36-155">DateTime the object was last modified.</span></span> <span data-ttu-id="60a36-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60a36-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="60a36-157">displayName</span><span class="sxs-lookup"><span data-stu-id="60a36-157">displayName</span></span>|<span data-ttu-id="60a36-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60a36-158">String</span></span>|<span data-ttu-id="60a36-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="60a36-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="60a36-160">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60a36-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="60a36-161">version</span><span class="sxs-lookup"><span data-stu-id="60a36-161">version</span></span>|<span data-ttu-id="60a36-162">Int32</span><span class="sxs-lookup"><span data-stu-id="60a36-162">Int32</span></span>|<span data-ttu-id="60a36-163">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="60a36-163">Version of the device configuration.</span></span> <span data-ttu-id="60a36-164">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60a36-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="60a36-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="60a36-165">encodedSettingXml</span></span>|<span data-ttu-id="60a36-166">Binary</span><span class="sxs-lookup"><span data-stu-id="60a36-166">Binary</span></span>|<span data-ttu-id="60a36-167">Base64-binärcodierte MDM-App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="60a36-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="60a36-168">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="60a36-168">settings</span></span>|<span data-ttu-id="60a36-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="60a36-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="60a36-170">App-Konfigurationseinstellungselemente</span><span class="sxs-lookup"><span data-stu-id="60a36-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="60a36-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="60a36-171">Response</span></span>
<span data-ttu-id="60a36-172">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="60a36-172">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60a36-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60a36-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="60a36-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60a36-174">Request</span></span>
<span data-ttu-id="60a36-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60a36-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 596

{
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="60a36-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="60a36-176">Response</span></span>
<span data-ttu-id="60a36-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60a36-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





