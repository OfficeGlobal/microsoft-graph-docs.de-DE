---
title: Auflisten von „iosDeviceFeaturesConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosDeviceFeaturesConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e302237c776ea3ef6a6326920b1dc876a16cdfa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957598"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="4ca50-103">Auflisten von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="4ca50-103">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="4ca50-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ca50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ca50-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4ca50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ca50-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="4ca50-106">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ca50-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4ca50-107">Prerequisites</span></span>
<span data-ttu-id="4ca50-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ca50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ca50-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ca50-110">Permission type</span></span>|<span data-ttu-id="4ca50-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ca50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ca50-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ca50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ca50-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ca50-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ca50-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ca50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ca50-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ca50-115">Not supported.</span></span>|
|<span data-ttu-id="4ca50-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ca50-116">Application</span></span>|<span data-ttu-id="4ca50-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ca50-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ca50-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ca50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ca50-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ca50-119">Request headers</span></span>
|<span data-ttu-id="4ca50-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4ca50-120">Header</span></span>|<span data-ttu-id="4ca50-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4ca50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ca50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ca50-122">Authorization</span></span>|<span data-ttu-id="4ca50-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4ca50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ca50-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4ca50-124">Accept</span></span>|<span data-ttu-id="4ca50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ca50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ca50-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ca50-126">Request body</span></span>
<span data-ttu-id="4ca50-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4ca50-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ca50-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ca50-128">Response</span></span>
<span data-ttu-id="4ca50-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4ca50-129">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ca50-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ca50-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ca50-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ca50-131">Request</span></span>
<span data-ttu-id="4ca50-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ca50-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4ca50-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ca50-133">Response</span></span>
<span data-ttu-id="4ca50-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ca50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




