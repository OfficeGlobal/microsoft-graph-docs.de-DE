---
title: Liste windowsUniversalAppXContainedApps
description: Listeneigenschaften und Beziehungen der WindowsUniversalAppXContainedApp-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: aa796ca7b32295f50fcaa901f31b71fbaa058be5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964158"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="a1307-103">Liste windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="a1307-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="a1307-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a1307-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1307-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1307-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1307-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a1307-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1307-107">Listeneigenschaften und Beziehungen der [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a1307-107">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1307-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a1307-108">Prerequisites</span></span>
<span data-ttu-id="a1307-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1307-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1307-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1307-111">Permission type</span></span>|<span data-ttu-id="a1307-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1307-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1307-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1307-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1307-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1307-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1307-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1307-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1307-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1307-116">Not supported.</span></span>|
|<span data-ttu-id="a1307-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1307-117">Application</span></span>|<span data-ttu-id="a1307-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1307-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1307-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1307-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="a1307-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1307-120">Request headers</span></span>
|<span data-ttu-id="a1307-121">Header</span><span class="sxs-lookup"><span data-stu-id="a1307-121">Header</span></span>|<span data-ttu-id="a1307-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a1307-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1307-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1307-123">Authorization</span></span>|<span data-ttu-id="a1307-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a1307-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1307-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a1307-125">Accept</span></span>|<span data-ttu-id="a1307-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1307-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1307-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1307-127">Request body</span></span>
<span data-ttu-id="a1307-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a1307-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1307-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1307-129">Response</span></span>
<span data-ttu-id="a1307-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a1307-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1307-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1307-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1307-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1307-132">Request</span></span>
<span data-ttu-id="a1307-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1307-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="a1307-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1307-134">Response</span></span>
<span data-ttu-id="a1307-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1307-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





