---
title: mobileAppContent abrufen
description: Lesen von Eigenschaften und Beziehungen des mobileAppContent-Objekts.
author: tfitzmac
ms.openlocfilehash: ab5c660f4bb5e505e70b7ae71211fcc8c3c69f18
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356525"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="6a462-103">mobileAppContent abrufen</span><span class="sxs-lookup"><span data-stu-id="6a462-103">Get mobileAppContent</span></span>

> <span data-ttu-id="6a462-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6a462-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a462-105">Lesen von Eigenschaften und Beziehungen des [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a462-105">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a462-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6a462-106">Prerequisites</span></span>
<span data-ttu-id="6a462-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a462-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a462-109">Permission type</span></span>|<span data-ttu-id="6a462-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a462-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a462-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a462-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a462-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a462-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6a462-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a462-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a462-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a462-114">Not supported.</span></span>|
|<span data-ttu-id="6a462-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a462-115">Application</span></span>|<span data-ttu-id="6a462-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a462-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a462-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a462-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a462-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6a462-118">Optional query parameters</span></span>
<span data-ttu-id="6a462-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6a462-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6a462-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a462-120">Request headers</span></span>
|<span data-ttu-id="6a462-121">Header</span><span class="sxs-lookup"><span data-stu-id="6a462-121">Header</span></span>|<span data-ttu-id="6a462-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6a462-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a462-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6a462-123">Authorization</span></span>|<span data-ttu-id="6a462-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6a462-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a462-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6a462-125">Accept</span></span>|<span data-ttu-id="6a462-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a462-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a462-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a462-127">Request body</span></span>
<span data-ttu-id="6a462-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6a462-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a462-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a462-129">Response</span></span>
<span data-ttu-id="6a462-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a462-130">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a462-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a462-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a462-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a462-132">Request</span></span>
<span data-ttu-id="6a462-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a462-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="6a462-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a462-134">Response</span></span>
<span data-ttu-id="6a462-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a462-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```



