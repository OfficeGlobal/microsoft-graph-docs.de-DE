---
title: Liste windowsKioskConfigurations
description: Listeneigenschaften und Beziehungen der WindowsKioskConfiguration-Objekte.
ms.openlocfilehash: bb178bca4c1ce11958e28ed8c5ad4fa23ad4d668
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065475"
---
# <a name="list-windowskioskconfigurations"></a><span data-ttu-id="3a20c-103">Liste windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="3a20c-103">List windowsKioskConfigurations</span></span>

> <span data-ttu-id="3a20c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3a20c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a20c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a20c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a20c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3a20c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a20c-107">Listeneigenschaften und Beziehungen der [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3a20c-107">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a20c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3a20c-108">Prerequisites</span></span>
<span data-ttu-id="3a20c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a20c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a20c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a20c-111">Permission type</span></span>|<span data-ttu-id="3a20c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a20c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a20c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a20c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a20c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a20c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3a20c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a20c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a20c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a20c-116">Not supported.</span></span>|
|<span data-ttu-id="3a20c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a20c-117">Application</span></span>|<span data-ttu-id="3a20c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a20c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a20c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a20c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3a20c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a20c-120">Request headers</span></span>
|<span data-ttu-id="3a20c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3a20c-121">Header</span></span>|<span data-ttu-id="3a20c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3a20c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a20c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a20c-123">Authorization</span></span>|<span data-ttu-id="3a20c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3a20c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a20c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a20c-125">Accept</span></span>|<span data-ttu-id="3a20c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a20c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a20c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a20c-127">Request body</span></span>
<span data-ttu-id="3a20c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3a20c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a20c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a20c-129">Response</span></span>
<span data-ttu-id="3a20c-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3a20c-130">If successful, this method returns a `200 OK` response code and a collection of [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a20c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a20c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a20c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a20c-132">Request</span></span>
<span data-ttu-id="3a20c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a20c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3a20c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a20c-134">Response</span></span>
<span data-ttu-id="3a20c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a20c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

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
      ]
    }
  ]
}
```





