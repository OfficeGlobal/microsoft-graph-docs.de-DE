---
title: Auflisten von „iosDeviceFeaturesConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosDeviceFeaturesConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 31a903c3d938b2f85227e7a5d0e51d3003f64727
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884112"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="c96fe-103">Auflisten von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="c96fe-103">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="c96fe-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c96fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c96fe-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="c96fe-105">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c96fe-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c96fe-106">Prerequisites</span></span>
<span data-ttu-id="c96fe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c96fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c96fe-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c96fe-109">Permission type</span></span>|<span data-ttu-id="c96fe-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c96fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c96fe-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c96fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c96fe-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c96fe-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c96fe-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c96fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c96fe-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c96fe-114">Not supported.</span></span>|
|<span data-ttu-id="c96fe-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c96fe-115">Application</span></span>|<span data-ttu-id="c96fe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c96fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c96fe-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c96fe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c96fe-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c96fe-118">Request headers</span></span>
|<span data-ttu-id="c96fe-119">Header</span><span class="sxs-lookup"><span data-stu-id="c96fe-119">Header</span></span>|<span data-ttu-id="c96fe-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c96fe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c96fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c96fe-121">Authorization</span></span>|<span data-ttu-id="c96fe-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c96fe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c96fe-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c96fe-123">Accept</span></span>|<span data-ttu-id="c96fe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c96fe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c96fe-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c96fe-125">Request body</span></span>
<span data-ttu-id="c96fe-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c96fe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c96fe-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c96fe-127">Response</span></span>
<span data-ttu-id="c96fe-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c96fe-128">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c96fe-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c96fe-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c96fe-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c96fe-130">Request</span></span>
<span data-ttu-id="c96fe-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c96fe-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c96fe-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c96fe-132">Response</span></span>
<span data-ttu-id="c96fe-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c96fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2461

{
  "value": [
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
  ]
}
```



