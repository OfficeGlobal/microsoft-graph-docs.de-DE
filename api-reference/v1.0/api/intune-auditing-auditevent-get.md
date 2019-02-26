---
title: Abrufen von „auditEvent“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a97f8e774d7f3ccb855ff8f9c923bbc8109581f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255122"
---
# <a name="get-auditevent"></a><span data-ttu-id="e563a-103">Abrufen von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="e563a-103">Get auditEvent</span></span>

> <span data-ttu-id="e563a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e563a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e563a-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="e563a-105">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e563a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e563a-106">Prerequisites</span></span>
<span data-ttu-id="e563a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e563a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e563a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e563a-109">Permission type</span></span>|<span data-ttu-id="e563a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e563a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e563a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e563a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e563a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e563a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e563a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e563a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e563a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e563a-114">Not supported.</span></span>|
|<span data-ttu-id="e563a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e563a-115">Application</span></span>|<span data-ttu-id="e563a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e563a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e563a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e563a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e563a-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e563a-118">Optional query parameters</span></span>
<span data-ttu-id="e563a-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e563a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e563a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e563a-120">Request headers</span></span>
|<span data-ttu-id="e563a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e563a-121">Header</span></span>|<span data-ttu-id="e563a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e563a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e563a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e563a-123">Authorization</span></span>|<span data-ttu-id="e563a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e563a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e563a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e563a-125">Accept</span></span>|<span data-ttu-id="e563a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e563a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e563a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e563a-127">Request body</span></span>
<span data-ttu-id="e563a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e563a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e563a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e563a-129">Response</span></span>
<span data-ttu-id="e563a-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e563a-130">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e563a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e563a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e563a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e563a-132">Request</span></span>
<span data-ttu-id="e563a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e563a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="e563a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e563a-134">Response</span></span>
<span data-ttu-id="e563a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e563a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



