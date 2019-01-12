---
title: Abrufen von „auditEvent“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 675a4c29c2efd73e14c11d1e7ce4ef6e6b0917c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920940"
---
# <a name="get-auditevent"></a><span data-ttu-id="a761a-103">Abrufen von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="a761a-103">Get auditEvent</span></span>

> <span data-ttu-id="a761a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a761a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a761a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a761a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a761a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a761a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a761a-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="a761a-107">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a761a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a761a-108">Prerequisites</span></span>
<span data-ttu-id="a761a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a761a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a761a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a761a-111">Permission type</span></span>|<span data-ttu-id="a761a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a761a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a761a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a761a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a761a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a761a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a761a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a761a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a761a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a761a-116">Not supported.</span></span>|
|<span data-ttu-id="a761a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a761a-117">Application</span></span>|<span data-ttu-id="a761a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a761a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a761a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a761a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a761a-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a761a-120">Optional query parameters</span></span>
<span data-ttu-id="a761a-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a761a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a761a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a761a-122">Request headers</span></span>
|<span data-ttu-id="a761a-123">Header</span><span class="sxs-lookup"><span data-stu-id="a761a-123">Header</span></span>|<span data-ttu-id="a761a-124">Wert</span><span class="sxs-lookup"><span data-stu-id="a761a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a761a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a761a-125">Authorization</span></span>|<span data-ttu-id="a761a-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a761a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a761a-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a761a-127">Accept</span></span>|<span data-ttu-id="a761a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a761a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a761a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a761a-129">Request body</span></span>
<span data-ttu-id="a761a-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a761a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a761a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a761a-131">Response</span></span>
<span data-ttu-id="a761a-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a761a-132">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a761a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a761a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a761a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a761a-134">Request</span></span>
<span data-ttu-id="a761a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a761a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="a761a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a761a-136">Response</span></span>
<span data-ttu-id="a761a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a761a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
    "@odata.type": "#microsoft.graph.auditEvent",
    "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
    "displayName": "Display Name value",
    "componentName": "Component Name value",
    "actor": {
      "@odata.type": "microsoft.graph.auditActor",
      "type": "Type value",
      "userPermissions": [
        "User Permissions value"
      ],
      "applicationId": "Application Id value",
      "applicationDisplayName": "Application Display Name value",
      "userPrincipalName": "User Principal Name value",
      "servicePrincipalName": "Service Principal Name value",
      "ipAddress": "Ip Address value",
      "userId": "User Id value"
    },
    "activity": "Activity value",
    "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
    "activityType": "Activity Type value",
    "activityOperationType": "Activity Operation Type value",
    "activityResult": "Activity Result value",
    "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
    "resources": [
      {
        "@odata.type": "microsoft.graph.auditResource",
        "displayName": "Display Name value",
        "modifiedProperties": [
          {
            "@odata.type": "microsoft.graph.auditProperty",
            "displayName": "Display Name value",
            "oldValue": "Old Value value",
            "newValue": "New Value value"
          }
        ],
        "type": "Type value",
        "resourceId": "Resource Id value"
      }
    ],
    "category": "Category value"
  }
}
```





