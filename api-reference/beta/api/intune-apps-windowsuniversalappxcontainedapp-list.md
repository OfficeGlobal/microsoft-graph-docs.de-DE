---
title: Liste windowsUniversalAppXContainedApps
description: Listeneigenschaften und Beziehungen der WindowsUniversalAppXContainedApp-Objekte.
ms.openlocfilehash: cfe51a97e09f446cb8241f739f5339e88c1041f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064519"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="acede-103">Liste windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="acede-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="acede-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="acede-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acede-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acede-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acede-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acede-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acede-107">Listeneigenschaften und Beziehungen der [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="acede-107">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acede-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="acede-108">Prerequisites</span></span>
<span data-ttu-id="acede-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acede-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acede-111">Permission type</span></span>|<span data-ttu-id="acede-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acede-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acede-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acede-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acede-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="acede-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="acede-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acede-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acede-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acede-116">Not supported.</span></span>|
|<span data-ttu-id="acede-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acede-117">Application</span></span>|<span data-ttu-id="acede-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acede-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acede-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acede-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="acede-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acede-120">Request headers</span></span>
|<span data-ttu-id="acede-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="acede-121">Header</span></span>|<span data-ttu-id="acede-122">Wert</span><span class="sxs-lookup"><span data-stu-id="acede-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acede-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acede-123">Authorization</span></span>|<span data-ttu-id="acede-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="acede-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acede-125">Accept</span><span class="sxs-lookup"><span data-stu-id="acede-125">Accept</span></span>|<span data-ttu-id="acede-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acede-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acede-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acede-127">Request body</span></span>
<span data-ttu-id="acede-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="acede-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acede-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="acede-129">Response</span></span>
<span data-ttu-id="acede-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="acede-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acede-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acede-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="acede-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acede-132">Request</span></span>
<span data-ttu-id="acede-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acede-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="acede-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="acede-134">Response</span></span>
<span data-ttu-id="acede-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acede-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
      "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
      "appUserModelId": "App User Model Id value"
    }
  ]
}
```





