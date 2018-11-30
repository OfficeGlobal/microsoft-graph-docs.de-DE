---
title: Auflisten von „webApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs webApp auf.
ms.openlocfilehash: 1114b2086ab1a1170eb49b67e8b38366d53db93b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065204"
---
# <a name="list-webapps"></a><span data-ttu-id="2592f-103">Auflisten von „webApp“</span><span class="sxs-lookup"><span data-stu-id="2592f-103">List webApps</span></span>

> <span data-ttu-id="2592f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2592f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2592f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2592f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2592f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2592f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2592f-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [webApp](../resources/intune-apps-webapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="2592f-107">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2592f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2592f-108">Prerequisites</span></span>
<span data-ttu-id="2592f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2592f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2592f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2592f-111">Permission type</span></span>|<span data-ttu-id="2592f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2592f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2592f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2592f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2592f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2592f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2592f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2592f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2592f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2592f-116">Not supported.</span></span>|
|<span data-ttu-id="2592f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2592f-117">Application</span></span>|<span data-ttu-id="2592f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2592f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2592f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2592f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2592f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2592f-120">Request headers</span></span>
|<span data-ttu-id="2592f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2592f-121">Header</span></span>|<span data-ttu-id="2592f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2592f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2592f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2592f-123">Authorization</span></span>|<span data-ttu-id="2592f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2592f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2592f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2592f-125">Accept</span></span>|<span data-ttu-id="2592f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2592f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2592f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2592f-127">Request body</span></span>
<span data-ttu-id="2592f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2592f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2592f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2592f-129">Response</span></span>
<span data-ttu-id="2592f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [webApp](../resources/intune-apps-webapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2592f-130">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2592f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2592f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2592f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2592f-132">Request</span></span>
<span data-ttu-id="2592f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2592f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2592f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2592f-134">Response</span></span>
<span data-ttu-id="2592f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2592f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 960

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.webApp",
      "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```





