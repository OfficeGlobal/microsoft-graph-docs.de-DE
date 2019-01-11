---
title: mobileAppAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des mobileAppAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 790b6e6a8c0f970c7f4b0aa13ed739cec585d9d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831122"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="56aee-103">mobileAppAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="56aee-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="56aee-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56aee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56aee-105">Lesen von Eigenschaften und Beziehungen des [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56aee-105">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56aee-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="56aee-106">Prerequisites</span></span>
<span data-ttu-id="56aee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56aee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56aee-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56aee-109">Permission type</span></span>|<span data-ttu-id="56aee-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56aee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56aee-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56aee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56aee-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="56aee-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="56aee-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56aee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56aee-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56aee-114">Not supported.</span></span>|
|<span data-ttu-id="56aee-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56aee-115">Application</span></span>|<span data-ttu-id="56aee-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56aee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56aee-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56aee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56aee-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="56aee-118">Optional query parameters</span></span>
<span data-ttu-id="56aee-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="56aee-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56aee-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56aee-120">Request headers</span></span>
|<span data-ttu-id="56aee-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="56aee-121">Header</span></span>|<span data-ttu-id="56aee-122">Wert</span><span class="sxs-lookup"><span data-stu-id="56aee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56aee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56aee-123">Authorization</span></span>|<span data-ttu-id="56aee-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="56aee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56aee-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="56aee-125">Accept</span></span>|<span data-ttu-id="56aee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56aee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56aee-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56aee-127">Request body</span></span>
<span data-ttu-id="56aee-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="56aee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56aee-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="56aee-129">Response</span></span>
<span data-ttu-id="56aee-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56aee-130">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56aee-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56aee-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="56aee-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56aee-132">Request</span></span>
<span data-ttu-id="56aee-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56aee-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="56aee-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="56aee-134">Response</span></span>
<span data-ttu-id="56aee-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56aee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppAssignment",
    "id": "591620b7-20b7-5916-b720-1659b7201659",
    "intent": "required",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "settings": {
      "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
    }
  }
}
```



