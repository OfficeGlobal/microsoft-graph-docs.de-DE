---
title: Auflisten von „windowsUniversalAppX“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsUniversalAppX auf.
ms.openlocfilehash: 54f943ccc312dc051593287f5567f39828547617
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016692"
---
# <a name="list-windowsuniversalappxs"></a><span data-ttu-id="aedbb-103">Auflisten von „windowsUniversalAppX“</span><span class="sxs-lookup"><span data-stu-id="aedbb-103">List windowsUniversalAppXs</span></span>

> <span data-ttu-id="aedbb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aedbb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aedbb-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) auf.</span><span class="sxs-lookup"><span data-stu-id="aedbb-105">List properties and relationships of the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aedbb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aedbb-106">Prerequisites</span></span>
<span data-ttu-id="aedbb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aedbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aedbb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aedbb-109">Permission type</span></span>|<span data-ttu-id="aedbb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aedbb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aedbb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aedbb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aedbb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aedbb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aedbb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aedbb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aedbb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aedbb-114">Not supported.</span></span>|
|<span data-ttu-id="aedbb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aedbb-115">Application</span></span>|<span data-ttu-id="aedbb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aedbb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aedbb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aedbb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="aedbb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aedbb-118">Request headers</span></span>
|<span data-ttu-id="aedbb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="aedbb-119">Header</span></span>|<span data-ttu-id="aedbb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="aedbb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aedbb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aedbb-121">Authorization</span></span>|<span data-ttu-id="aedbb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aedbb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aedbb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="aedbb-123">Accept</span></span>|<span data-ttu-id="aedbb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aedbb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aedbb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aedbb-125">Request body</span></span>
<span data-ttu-id="aedbb-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aedbb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aedbb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="aedbb-127">Response</span></span>
<span data-ttu-id="aedbb-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aedbb-128">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aedbb-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aedbb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="aedbb-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aedbb-130">Request</span></span>
<span data-ttu-id="aedbb-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aedbb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="aedbb-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="aedbb-132">Response</span></span>
<span data-ttu-id="aedbb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aedbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1534

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUniversalAppX",
      "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "applicableArchitectures": "x86",
      "applicableDeviceTypes": "desktop",
      "identityName": "Identity Name value",
      "identityPublisherHash": "Identity Publisher Hash value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "isBundle": true,
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true
      },
      "identityVersion": "Identity Version value"
    }
  ]
}
```


