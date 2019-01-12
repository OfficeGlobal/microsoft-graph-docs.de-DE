---
title: Erstellen von „iosDeviceFeaturesConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 46f82069cabad946613b3929d378974a9b3dc642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957522"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="8f369-103">Erstellen von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="8f369-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="8f369-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8f369-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f369-105">Diese Methode erstellt ein neues Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f369-105">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f369-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8f369-106">Prerequisites</span></span>
<span data-ttu-id="8f369-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f369-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f369-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8f369-109">Permission type</span></span>|<span data-ttu-id="8f369-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8f369-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f369-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8f369-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f369-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f369-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f369-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8f369-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f369-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f369-114">Not supported.</span></span>|
|<span data-ttu-id="8f369-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8f369-115">Application</span></span>|<span data-ttu-id="8f369-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f369-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f369-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f369-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8f369-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8f369-118">Request headers</span></span>
|<span data-ttu-id="8f369-119">Header</span><span class="sxs-lookup"><span data-stu-id="8f369-119">Header</span></span>|<span data-ttu-id="8f369-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8f369-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f369-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f369-121">Authorization</span></span>|<span data-ttu-id="8f369-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8f369-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f369-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8f369-123">Accept</span></span>|<span data-ttu-id="8f369-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f369-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f369-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8f369-125">Request body</span></span>
<span data-ttu-id="8f369-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="8f369-126">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="8f369-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="8f369-127">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="8f369-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f369-128">Property</span></span>|<span data-ttu-id="8f369-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8f369-129">Type</span></span>|<span data-ttu-id="8f369-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f369-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f369-131">id</span><span class="sxs-lookup"><span data-stu-id="8f369-131">id</span></span>|<span data-ttu-id="8f369-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f369-132">String</span></span>|<span data-ttu-id="8f369-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8f369-133">Key of the entity.</span></span> <span data-ttu-id="8f369-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f369-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f369-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f369-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8f369-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f369-136">DateTimeOffset</span></span>|<span data-ttu-id="8f369-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f369-137">DateTime the object was last modified.</span></span> <span data-ttu-id="8f369-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f369-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f369-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f369-139">createdDateTime</span></span>|<span data-ttu-id="8f369-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f369-140">DateTimeOffset</span></span>|<span data-ttu-id="8f369-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f369-141">DateTime the object was created.</span></span> <span data-ttu-id="8f369-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f369-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f369-143">description</span><span class="sxs-lookup"><span data-stu-id="8f369-143">description</span></span>|<span data-ttu-id="8f369-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f369-144">String</span></span>|<span data-ttu-id="8f369-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8f369-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f369-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f369-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f369-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8f369-147">displayName</span></span>|<span data-ttu-id="8f369-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f369-148">String</span></span>|<span data-ttu-id="8f369-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8f369-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f369-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f369-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f369-151">Version</span><span class="sxs-lookup"><span data-stu-id="8f369-151">version</span></span>|<span data-ttu-id="8f369-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8f369-152">Int32</span></span>|<span data-ttu-id="8f369-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8f369-153">Version of the device configuration.</span></span> <span data-ttu-id="8f369-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f369-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f369-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="8f369-155">assetTagTemplate</span></span>|<span data-ttu-id="8f369-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f369-156">String</span></span>|<span data-ttu-id="8f369-157">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8f369-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="8f369-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="8f369-158">lockScreenFootnote</span></span>|<span data-ttu-id="8f369-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f369-159">String</span></span>|<span data-ttu-id="8f369-160">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="8f369-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="8f369-161">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="8f369-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="8f369-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="8f369-162">homeScreenDockIcons</span></span>|<span data-ttu-id="8f369-163">Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8f369-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="8f369-164">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8f369-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="8f369-165">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="8f369-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8f369-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="8f369-166">homeScreenPages</span></span>|<span data-ttu-id="8f369-167">Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="8f369-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="8f369-168">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="8f369-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="8f369-169">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="8f369-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8f369-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="8f369-170">notificationSettings</span></span>|<span data-ttu-id="8f369-171">Collection von Objekten des Typs [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8f369-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="8f369-172">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="8f369-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="8f369-173">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="8f369-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8f369-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f369-174">Response</span></span>
<span data-ttu-id="8f369-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8f369-175">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f369-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8f369-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f369-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f369-177">Request</span></span>
<span data-ttu-id="8f369-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8f369-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="8f369-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f369-179">Response</span></span>
<span data-ttu-id="8f369-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f369-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```



