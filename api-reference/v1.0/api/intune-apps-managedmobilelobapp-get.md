---
title: managedMobileLobApp abrufen
description: Lesen von Eigenschaften und Beziehungen des managedMobileLobApp-Objekts.
author: tfitzmac
ms.openlocfilehash: b15f4337c8ff5669d50ada9335f1fde7b111f205
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325466"
---
# <a name="get-managedmobilelobapp"></a><span data-ttu-id="11cff-103">managedMobileLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="11cff-103">Get managedMobileLobApp</span></span>

> <span data-ttu-id="11cff-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="11cff-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11cff-105">Lesen von Eigenschaften und Beziehungen des [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="11cff-105">Read properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11cff-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="11cff-106">Prerequisites</span></span>
<span data-ttu-id="11cff-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11cff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11cff-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11cff-109">Permission type</span></span>|<span data-ttu-id="11cff-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11cff-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11cff-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11cff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11cff-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="11cff-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="11cff-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11cff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11cff-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11cff-114">Not supported.</span></span>|
|<span data-ttu-id="11cff-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11cff-115">Application</span></span>|<span data-ttu-id="11cff-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11cff-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11cff-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11cff-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11cff-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="11cff-118">Optional query parameters</span></span>
<span data-ttu-id="11cff-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11cff-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="11cff-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11cff-120">Request headers</span></span>
|<span data-ttu-id="11cff-121">Header</span><span class="sxs-lookup"><span data-stu-id="11cff-121">Header</span></span>|<span data-ttu-id="11cff-122">Wert</span><span class="sxs-lookup"><span data-stu-id="11cff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11cff-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="11cff-123">Authorization</span></span>|<span data-ttu-id="11cff-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="11cff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11cff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="11cff-125">Accept</span></span>|<span data-ttu-id="11cff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11cff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11cff-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11cff-127">Request body</span></span>
<span data-ttu-id="11cff-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="11cff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11cff-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="11cff-129">Response</span></span>
<span data-ttu-id="11cff-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11cff-130">If successful, this method returns a `200 OK` response code and [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11cff-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11cff-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="11cff-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11cff-132">Request</span></span>
<span data-ttu-id="11cff-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11cff-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="11cff-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="11cff-134">Response</span></span>
<span data-ttu-id="11cff-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11cff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1007

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
    "publishingState": "processing",
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```



