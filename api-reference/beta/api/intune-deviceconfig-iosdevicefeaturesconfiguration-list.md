---
title: Auflisten von „iosDeviceFeaturesConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosDeviceFeaturesConfiguration auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f72ca3b336e200ffd61976348e567d2bf1a3c05b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404533"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="45e7f-103">Auflisten von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="45e7f-103">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="45e7f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="45e7f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45e7f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="45e7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45e7f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45e7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45e7f-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="45e7f-107">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45e7f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="45e7f-108">Prerequisites</span></span>
<span data-ttu-id="45e7f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="45e7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="45e7f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45e7f-111">Permission type</span></span>|<span data-ttu-id="45e7f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45e7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45e7f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45e7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45e7f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45e7f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45e7f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45e7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45e7f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45e7f-116">Not supported.</span></span>|
|<span data-ttu-id="45e7f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45e7f-117">Application</span></span>|<span data-ttu-id="45e7f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45e7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45e7f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45e7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45e7f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45e7f-120">Request headers</span></span>
|<span data-ttu-id="45e7f-121">Header</span><span class="sxs-lookup"><span data-stu-id="45e7f-121">Header</span></span>|<span data-ttu-id="45e7f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="45e7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45e7f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="45e7f-123">Authorization</span></span>|<span data-ttu-id="45e7f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="45e7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45e7f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="45e7f-125">Accept</span></span>|<span data-ttu-id="45e7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45e7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45e7f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45e7f-127">Request body</span></span>
<span data-ttu-id="45e7f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="45e7f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45e7f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="45e7f-129">Response</span></span>
<span data-ttu-id="45e7f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="45e7f-130">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45e7f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45e7f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45e7f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45e7f-132">Request</span></span>
<span data-ttu-id="45e7f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45e7f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="45e7f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="45e7f-134">Response</span></span>
<span data-ttu-id="45e7f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45e7f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4353

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
      "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "airPrintDestinations": [
        {
          "@odata.type": "microsoft.graph.airPrintDestination",
          "ipAddress": "Ip Address value",
          "resourcePath": "Resource Path value",
          "port": 4,
          "forceTls": true
        }
      ],
      "assetTagTemplate": "Asset Tag Template value",
      "contentFilterSettings": {
        "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
        "specificWebsitesOnly": [
          {
            "@odata.type": "microsoft.graph.iosBookmark",
            "url": "Url value",
            "bookmarkFolder": "Bookmark Folder value",
            "displayName": "Display Name value"
          }
        ],
        "websiteList": [
          {
            "@odata.type": "microsoft.graph.iosBookmark",
            "url": "Url value",
            "bookmarkFolder": "Bookmark Folder value",
            "displayName": "Display Name value"
          }
        ]
      },
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
      ],
      "singleSignOnSettings": {
        "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
        "allowedAppsList": [
          {
            "@odata.type": "microsoft.graph.appListItem",
            "name": "Name value",
            "publisher": "Publisher value",
            "appStoreUrl": "https://example.com/appStoreUrl/",
            "appId": "App Id value"
          }
        ],
        "allowedUrls": [
          "Allowed Urls value"
        ],
        "displayName": "Display Name value",
        "kerberosPrincipalName": "Kerberos Principal Name value",
        "kerberosRealm": "Kerberos Realm value"
      },
      "wallpaperDisplayLocation": "lockScreen",
      "wallpaperImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ]
}
```




