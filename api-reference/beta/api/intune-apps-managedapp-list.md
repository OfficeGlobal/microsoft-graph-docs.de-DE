---
title: Auflisten von „managedApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedApp auf.
ms.openlocfilehash: 33b91220d034c3b24db471ea8800934c6907100a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062333"
---
# <a name="list-managedapps"></a><span data-ttu-id="12fe7-103">Auflisten von „managedApp“</span><span class="sxs-lookup"><span data-stu-id="12fe7-103">List managedApps</span></span>

> <span data-ttu-id="12fe7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12fe7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12fe7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12fe7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12fe7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="12fe7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12fe7-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedApp](../resources/intune-apps-managedapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="12fe7-107">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12fe7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="12fe7-108">Prerequisites</span></span>
<span data-ttu-id="12fe7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fe7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12fe7-111">Permission type</span></span>|<span data-ttu-id="12fe7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12fe7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12fe7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12fe7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12fe7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="12fe7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="12fe7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12fe7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12fe7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12fe7-116">Not supported.</span></span>|
|<span data-ttu-id="12fe7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12fe7-117">Application</span></span>|<span data-ttu-id="12fe7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12fe7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12fe7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fe7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="12fe7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12fe7-120">Request headers</span></span>
|<span data-ttu-id="12fe7-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="12fe7-121">Header</span></span>|<span data-ttu-id="12fe7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="12fe7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12fe7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12fe7-123">Authorization</span></span>|<span data-ttu-id="12fe7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="12fe7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12fe7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12fe7-125">Accept</span></span>|<span data-ttu-id="12fe7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12fe7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fe7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12fe7-127">Request body</span></span>
<span data-ttu-id="12fe7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="12fe7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12fe7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fe7-129">Response</span></span>
<span data-ttu-id="12fe7-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedApp](../resources/intune-apps-managedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="12fe7-130">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12fe7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12fe7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="12fe7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fe7-132">Request</span></span>
<span data-ttu-id="12fe7-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="12fe7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="12fe7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fe7-134">Response</span></span>
<span data-ttu-id="12fe7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fe7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 961

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedApp",
      "id": "f687dd85-dd85-f687-85dd-87f685dd87f6",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value"
    }
  ]
}
```





