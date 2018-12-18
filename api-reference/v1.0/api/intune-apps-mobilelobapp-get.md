---
title: mobileLobApp abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des mobileLobApp-Objekts auf.
author: tfitzmac
ms.openlocfilehash: d94e4b89b481b0b567b92b35f19f71473393fe53
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333362"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="ddc46-103">mobileLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="ddc46-103">Get mobileLobApp</span></span>

> <span data-ttu-id="ddc46-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ddc46-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddc46-105">Liest die Eigenschaften und Beziehungen von Objekten des [mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="ddc46-105">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddc46-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ddc46-106">Prerequisites</span></span>
<span data-ttu-id="ddc46-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddc46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddc46-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ddc46-109">Permission type</span></span>|<span data-ttu-id="ddc46-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ddc46-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddc46-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ddc46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ddc46-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddc46-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ddc46-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ddc46-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddc46-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ddc46-114">Not supported.</span></span>|
|<span data-ttu-id="ddc46-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ddc46-115">Application</span></span>|<span data-ttu-id="ddc46-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ddc46-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddc46-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ddc46-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddc46-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ddc46-118">Optional query parameters</span></span>
<span data-ttu-id="ddc46-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ddc46-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ddc46-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ddc46-120">Request headers</span></span>
|<span data-ttu-id="ddc46-121">Header</span><span class="sxs-lookup"><span data-stu-id="ddc46-121">Header</span></span>|<span data-ttu-id="ddc46-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ddc46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddc46-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ddc46-123">Authorization</span></span>|<span data-ttu-id="ddc46-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ddc46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddc46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ddc46-125">Accept</span></span>|<span data-ttu-id="ddc46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddc46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddc46-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ddc46-127">Request body</span></span>
<span data-ttu-id="ddc46-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ddc46-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddc46-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ddc46-129">Response</span></span>
<span data-ttu-id="ddc46-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ddc46-130">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddc46-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ddc46-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddc46-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ddc46-132">Request</span></span>
<span data-ttu-id="ddc46-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ddc46-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ddc46-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ddc46-134">Response</span></span>
<span data-ttu-id="ddc46-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ddc46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileLobApp",
    "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
    "size": 4
  }
}
```



