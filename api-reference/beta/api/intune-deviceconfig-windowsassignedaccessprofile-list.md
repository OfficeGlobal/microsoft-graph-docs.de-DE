---
title: Liste windowsAssignedAccessProfiles
description: Listeneigenschaften und Beziehungen der WindowsAssignedAccessProfile-Objekte.
ms.openlocfilehash: a8fdd5ce2aaba01f6e08f93326839847f63ff6bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062930"
---
# <a name="list-windowsassignedaccessprofiles"></a><span data-ttu-id="6ecf0-103">Liste windowsAssignedAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="6ecf0-103">List windowsAssignedAccessProfiles</span></span>

> <span data-ttu-id="6ecf0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ecf0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ecf0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ecf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ecf0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6ecf0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ecf0-107">Listeneigenschaften und Beziehungen der [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6ecf0-107">List properties and relationships of the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ecf0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6ecf0-108">Prerequisites</span></span>
<span data-ttu-id="6ecf0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ecf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ecf0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6ecf0-111">Permission type</span></span>|<span data-ttu-id="6ecf0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6ecf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ecf0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6ecf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ecf0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ecf0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6ecf0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6ecf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ecf0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ecf0-116">Not supported.</span></span>|
|<span data-ttu-id="6ecf0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6ecf0-117">Application</span></span>|<span data-ttu-id="6ecf0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ecf0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ecf0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ecf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6ecf0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6ecf0-120">Request headers</span></span>
|<span data-ttu-id="6ecf0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6ecf0-121">Header</span></span>|<span data-ttu-id="6ecf0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6ecf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ecf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ecf0-123">Authorization</span></span>|<span data-ttu-id="6ecf0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6ecf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ecf0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6ecf0-125">Accept</span></span>|<span data-ttu-id="6ecf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ecf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ecf0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6ecf0-127">Request body</span></span>
<span data-ttu-id="6ecf0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6ecf0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ecf0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ecf0-129">Response</span></span>
<span data-ttu-id="6ecf0-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6ecf0-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ecf0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6ecf0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ecf0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ecf0-132">Request</span></span>
<span data-ttu-id="6ecf0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6ecf0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
```

### <a name="response"></a><span data-ttu-id="6ecf0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ecf0-134">Response</span></span>
<span data-ttu-id="6ecf0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6ecf0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
      "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
      "profileName": "Profile Name value",
      "showTaskBar": true,
      "appUserModelIds": [
        "App User Model Ids value"
      ],
      "desktopAppPaths": [
        "Desktop App Paths value"
      ],
      "userAccounts": [
        "User Accounts value"
      ],
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
    }
  ]
}
```





