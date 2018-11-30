---
title: mobileLobApp abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des mobileLobApp-Objekts auf.
ms.openlocfilehash: fea0e895752016caa640ba6ceefab2f28c977be4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065158"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="3c191-103">mobileLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="3c191-103">Get mobileLobApp</span></span>

> <span data-ttu-id="3c191-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3c191-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c191-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c191-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c191-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3c191-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c191-107">Liest die Eigenschaften und Beziehungen von Objekten des [mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="3c191-107">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c191-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3c191-108">Prerequisites</span></span>
<span data-ttu-id="3c191-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c191-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c191-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c191-111">Permission type</span></span>|<span data-ttu-id="3c191-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c191-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c191-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c191-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c191-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c191-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3c191-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c191-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c191-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c191-116">Not supported.</span></span>|
|<span data-ttu-id="3c191-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c191-117">Application</span></span>|<span data-ttu-id="3c191-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c191-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c191-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c191-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c191-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3c191-120">Optional query parameters</span></span>
<span data-ttu-id="3c191-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3c191-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3c191-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3c191-122">Request headers</span></span>
|<span data-ttu-id="3c191-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3c191-123">Header</span></span>|<span data-ttu-id="3c191-124">Wert</span><span class="sxs-lookup"><span data-stu-id="3c191-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c191-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c191-125">Authorization</span></span>|<span data-ttu-id="3c191-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3c191-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c191-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3c191-127">Accept</span></span>|<span data-ttu-id="3c191-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3c191-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c191-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3c191-129">Request body</span></span>
<span data-ttu-id="3c191-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3c191-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c191-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c191-131">Response</span></span>
<span data-ttu-id="3c191-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c191-132">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c191-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3c191-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c191-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c191-134">Request</span></span>
<span data-ttu-id="3c191-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3c191-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3c191-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c191-136">Response</span></span>
<span data-ttu-id="3c191-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c191-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 949

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
    "uploadState": 11,
    "publishingState": "processing",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```





