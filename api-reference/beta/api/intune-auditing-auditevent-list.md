---
title: Auflisten von „auditEvent“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs auditEvent auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b16ddbf9a4b110afe172ced3ba9fdccc52b8e80c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409538"
---
# <a name="list-auditevents"></a><span data-ttu-id="02bc4-103">Auflisten von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="02bc4-103">List auditEvents</span></span>

> <span data-ttu-id="02bc4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="02bc4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="02bc4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02bc4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02bc4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02bc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02bc4-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [auditEvent](../resources/intune-auditing-auditevent.md) auf.</span><span class="sxs-lookup"><span data-stu-id="02bc4-107">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02bc4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="02bc4-108">Prerequisites</span></span>
<span data-ttu-id="02bc4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="02bc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="02bc4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02bc4-111">Permission type</span></span>|<span data-ttu-id="02bc4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02bc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02bc4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02bc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02bc4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02bc4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="02bc4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02bc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02bc4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02bc4-116">Not supported.</span></span>|
|<span data-ttu-id="02bc4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02bc4-117">Application</span></span>|<span data-ttu-id="02bc4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02bc4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02bc4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02bc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="02bc4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02bc4-120">Request headers</span></span>
|<span data-ttu-id="02bc4-121">Header</span><span class="sxs-lookup"><span data-stu-id="02bc4-121">Header</span></span>|<span data-ttu-id="02bc4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="02bc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02bc4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="02bc4-123">Authorization</span></span>|<span data-ttu-id="02bc4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="02bc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02bc4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="02bc4-125">Accept</span></span>|<span data-ttu-id="02bc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02bc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02bc4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02bc4-127">Request body</span></span>
<span data-ttu-id="02bc4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="02bc4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02bc4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="02bc4-129">Response</span></span>
<span data-ttu-id="02bc4-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="02bc4-130">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02bc4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02bc4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="02bc4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02bc4-132">Request</span></span>
<span data-ttu-id="02bc4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02bc4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="02bc4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="02bc4-134">Response</span></span>
<span data-ttu-id="02bc4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02bc4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1632

{
  "value": [
    {
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
  ]
}
```




