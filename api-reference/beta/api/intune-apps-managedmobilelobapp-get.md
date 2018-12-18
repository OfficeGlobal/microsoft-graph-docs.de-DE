---
title: managedMobileLobApp abrufen
description: Lesen von Eigenschaften und Beziehungen des managedMobileLobApp-Objekts.
author: tfitzmac
ms.openlocfilehash: b29a1cc20b5957c0dd26d6c7cd8e20c1027b03cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311445"
---
# <a name="get-managedmobilelobapp"></a><span data-ttu-id="ec642-103">managedMobileLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="ec642-103">Get managedMobileLobApp</span></span>

> <span data-ttu-id="ec642-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec642-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec642-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec642-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec642-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ec642-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec642-107">Lesen von Eigenschaften und Beziehungen des [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ec642-107">Read properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec642-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ec642-108">Prerequisites</span></span>
<span data-ttu-id="ec642-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec642-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec642-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec642-111">Permission type</span></span>|<span data-ttu-id="ec642-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec642-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec642-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec642-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec642-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec642-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ec642-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec642-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec642-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec642-116">Not supported.</span></span>|
|<span data-ttu-id="ec642-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec642-117">Application</span></span>|<span data-ttu-id="ec642-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec642-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec642-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec642-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec642-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ec642-120">Optional query parameters</span></span>
<span data-ttu-id="ec642-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ec642-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ec642-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec642-122">Request headers</span></span>
|<span data-ttu-id="ec642-123">Header</span><span class="sxs-lookup"><span data-stu-id="ec642-123">Header</span></span>|<span data-ttu-id="ec642-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ec642-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec642-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ec642-125">Authorization</span></span>|<span data-ttu-id="ec642-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ec642-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec642-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ec642-127">Accept</span></span>|<span data-ttu-id="ec642-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ec642-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec642-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec642-129">Request body</span></span>
<span data-ttu-id="ec642-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ec642-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec642-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec642-131">Response</span></span>
<span data-ttu-id="ec642-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec642-132">If successful, this method returns a `200 OK` response code and [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec642-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec642-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec642-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec642-134">Request</span></span>
<span data-ttu-id="ec642-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec642-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ec642-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec642-136">Response</span></span>
<span data-ttu-id="ec642-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec642-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1031

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileLobApp",
    "id": "cded7cc4-7cc4-cded-c47c-edcdc47cedcd",
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
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```





