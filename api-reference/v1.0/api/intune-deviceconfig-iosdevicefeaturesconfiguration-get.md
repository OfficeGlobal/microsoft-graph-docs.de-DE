---
title: Abrufen von „iosDeviceFeaturesConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9e54c836033db07dbce21638f889db8360a3822
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250019"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="6feb9-103">Abrufen von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="6feb9-103">Get iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6feb9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6feb9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6feb9-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6feb9-105">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6feb9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6feb9-106">Prerequisites</span></span>
<span data-ttu-id="6feb9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6feb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6feb9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6feb9-109">Permission type</span></span>|<span data-ttu-id="6feb9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6feb9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6feb9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6feb9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6feb9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6feb9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6feb9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6feb9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6feb9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6feb9-114">Not supported.</span></span>|
|<span data-ttu-id="6feb9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6feb9-115">Application</span></span>|<span data-ttu-id="6feb9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6feb9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6feb9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6feb9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6feb9-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6feb9-118">Optional query parameters</span></span>
<span data-ttu-id="6feb9-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6feb9-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6feb9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6feb9-120">Request headers</span></span>
|<span data-ttu-id="6feb9-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6feb9-121">Header</span></span>|<span data-ttu-id="6feb9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6feb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6feb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6feb9-123">Authorization</span></span>|<span data-ttu-id="6feb9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6feb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6feb9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6feb9-125">Accept</span></span>|<span data-ttu-id="6feb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6feb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6feb9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6feb9-127">Request body</span></span>
<span data-ttu-id="6feb9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6feb9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6feb9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6feb9-129">Response</span></span>
<span data-ttu-id="6feb9-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6feb9-130">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6feb9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6feb9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6feb9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6feb9-132">Request</span></span>
<span data-ttu-id="6feb9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6feb9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6feb9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6feb9-134">Response</span></span>
<span data-ttu-id="6feb9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6feb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": {
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
}
```



