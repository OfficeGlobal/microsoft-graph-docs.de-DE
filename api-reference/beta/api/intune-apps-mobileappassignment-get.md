---
title: mobileAppAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des mobileAppAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fb6161e1349466bb74cafefef596b30b82a4e9e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808395"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="d4125-103">mobileAppAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="d4125-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="d4125-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d4125-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4125-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4125-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4125-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d4125-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4125-107">Lesen von Eigenschaften und Beziehungen des [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4125-107">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4125-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4125-108">Prerequisites</span></span>
<span data-ttu-id="d4125-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4125-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4125-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4125-111">Permission type</span></span>|<span data-ttu-id="d4125-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4125-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4125-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4125-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4125-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4125-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d4125-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4125-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4125-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4125-116">Not supported.</span></span>|
|<span data-ttu-id="d4125-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4125-117">Application</span></span>|<span data-ttu-id="d4125-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4125-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4125-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4125-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4125-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d4125-120">Optional query parameters</span></span>
<span data-ttu-id="d4125-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d4125-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d4125-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4125-122">Request headers</span></span>
|<span data-ttu-id="d4125-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d4125-123">Header</span></span>|<span data-ttu-id="d4125-124">Wert</span><span class="sxs-lookup"><span data-stu-id="d4125-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4125-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4125-125">Authorization</span></span>|<span data-ttu-id="d4125-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4125-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4125-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4125-127">Accept</span></span>|<span data-ttu-id="d4125-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d4125-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4125-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4125-129">Request body</span></span>
<span data-ttu-id="d4125-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d4125-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4125-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4125-131">Response</span></span>
<span data-ttu-id="d4125-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4125-132">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4125-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4125-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4125-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4125-134">Request</span></span>
<span data-ttu-id="d4125-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4125-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d4125-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4125-136">Response</span></span>
<span data-ttu-id="d4125-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4125-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





