---
title: Auflisten von „webApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs webApp auf.
author: tfitzmac
ms.openlocfilehash: 8170786b5bd3bf8af5276c40674a8e7e8d8bf664
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328322"
---
# <a name="list-webapps"></a><span data-ttu-id="eb741-103">Auflisten von „webApp“</span><span class="sxs-lookup"><span data-stu-id="eb741-103">List webApps</span></span>

> <span data-ttu-id="eb741-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb741-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb741-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [webApp](../resources/intune-apps-webapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="eb741-105">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb741-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb741-106">Prerequisites</span></span>
<span data-ttu-id="eb741-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb741-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb741-109">Permission type</span></span>|<span data-ttu-id="eb741-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb741-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb741-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb741-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb741-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb741-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eb741-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb741-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb741-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb741-114">Not supported.</span></span>|
|<span data-ttu-id="eb741-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb741-115">Application</span></span>|<span data-ttu-id="eb741-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb741-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb741-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb741-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="eb741-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb741-118">Request headers</span></span>
|<span data-ttu-id="eb741-119">Header</span><span class="sxs-lookup"><span data-stu-id="eb741-119">Header</span></span>|<span data-ttu-id="eb741-120">Wert</span><span class="sxs-lookup"><span data-stu-id="eb741-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb741-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="eb741-121">Authorization</span></span>|<span data-ttu-id="eb741-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb741-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb741-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eb741-123">Accept</span></span>|<span data-ttu-id="eb741-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eb741-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb741-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb741-125">Request body</span></span>
<span data-ttu-id="eb741-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eb741-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb741-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb741-127">Response</span></span>
<span data-ttu-id="eb741-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [webApp](../resources/intune-apps-webapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eb741-128">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb741-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb741-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb741-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb741-130">Request</span></span>
<span data-ttu-id="eb741-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb741-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="eb741-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb741-132">Response</span></span>
<span data-ttu-id="eb741-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb741-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 934

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
      "publishingState": "processing",
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```



