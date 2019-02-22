---
title: WindowsKioskConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der windowsKioskConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c052ee390fe451c22cdbe047fb99bd1cbeaa97a4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168838"
---
# <a name="list-windowskioskconfigurations"></a><span data-ttu-id="1f982-103">WindowsKioskConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="1f982-103">List windowsKioskConfigurations</span></span>

> <span data-ttu-id="1f982-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f982-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f982-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1f982-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f982-106">AufListen von Eigenschaften und Beziehungen der [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="1f982-106">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f982-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1f982-107">Prerequisites</span></span>
<span data-ttu-id="1f982-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1f982-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f982-110">Permission type</span></span>|<span data-ttu-id="1f982-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f982-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f982-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f982-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f982-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f982-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1f982-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f982-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f982-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f982-115">Not supported.</span></span>|
|<span data-ttu-id="1f982-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f982-116">Application</span></span>|<span data-ttu-id="1f982-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f982-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f982-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f982-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1f982-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f982-119">Request headers</span></span>
|<span data-ttu-id="1f982-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1f982-120">Header</span></span>|<span data-ttu-id="1f982-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1f982-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f982-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f982-122">Authorization</span></span>|<span data-ttu-id="1f982-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1f982-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f982-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1f982-124">Accept</span></span>|<span data-ttu-id="1f982-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f982-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f982-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f982-126">Request body</span></span>
<span data-ttu-id="1f982-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1f982-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f982-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f982-128">Response</span></span>
<span data-ttu-id="1f982-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1f982-129">If successful, this method returns a `200 OK` response code and a collection of [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f982-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f982-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f982-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f982-131">Request</span></span>
<span data-ttu-id="1f982-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f982-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1f982-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f982-133">Response</span></span>
<span data-ttu-id="1f982-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f982-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
      "id": "146a990b-990b-146a-0b99-6a140b996a14",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "kioskProfiles": [
        {
          "@odata.type": "microsoft.graph.windowsKioskProfile",
          "profileId": "Profile Id value",
          "profileName": "Profile Name value",
          "appConfiguration": {
            "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
            "apps": [
              {
                "@odata.type": "microsoft.graph.windowsKioskUWPApp",
                "startLayoutTileSize": "small",
                "name": "Name value",
                "appType": "store",
                "appUserModelId": "App User Model Id value",
                "appId": "App Id value",
                "containedAppId": "Contained App Id value"
              }
            ],
            "showTaskBar": true,
            "disallowDesktopApps": true,
            "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
          },
          "userAccountsConfiguration": [
            {
              "@odata.type": "microsoft.graph.windowsKioskVisitor"
            }
          ]
        }
      ],
      "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
      "kioskBrowserEnableHomeButton": true,
      "kioskBrowserEnableNavigationButtons": true,
      "kioskBrowserEnableEndSessionButton": true,
      "kioskBrowserRestartOnIdleTimeInMinutes": 6,
      "kioskBrowserBlockedURLs": [
        "Kiosk Browser Blocked URLs value"
      ],
      "kioskBrowserBlockedUrlExceptions": [
        "Kiosk Browser Blocked Url Exceptions value"
      ],
      "edgeKioskEnablePublicBrowsing": true,
      "edgeKioskResetAfterIdleTimeInMinutes": 4
    }
  ]
}
```




