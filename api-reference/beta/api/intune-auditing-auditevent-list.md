---
title: Auflisten von „auditEvent“
description: Auflisten von Eigenschaften und Beziehungen der auditEvent-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e730a605e65af74666d0baa4b7a5ed2f04f781
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959383"
---
# <a name="list-auditevents"></a><span data-ttu-id="77892-103">Auflisten von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="77892-103">List auditEvents</span></span>

> <span data-ttu-id="77892-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77892-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77892-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77892-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77892-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [auditEvent](../resources/intune-auditing-auditevent.md) auf.</span><span class="sxs-lookup"><span data-stu-id="77892-106">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77892-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77892-107">Prerequisites</span></span>
<span data-ttu-id="77892-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77892-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77892-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77892-110">Permission type</span></span>|<span data-ttu-id="77892-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77892-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77892-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77892-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77892-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77892-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="77892-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77892-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77892-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77892-115">Not supported.</span></span>|
|<span data-ttu-id="77892-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77892-116">Application</span></span>|<span data-ttu-id="77892-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77892-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77892-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77892-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="77892-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77892-119">Request headers</span></span>
|<span data-ttu-id="77892-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77892-120">Header</span></span>|<span data-ttu-id="77892-121">Wert</span><span class="sxs-lookup"><span data-stu-id="77892-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77892-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77892-122">Authorization</span></span>|<span data-ttu-id="77892-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77892-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77892-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="77892-124">Accept</span></span>|<span data-ttu-id="77892-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77892-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77892-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77892-126">Request body</span></span>
<span data-ttu-id="77892-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="77892-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77892-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="77892-128">Response</span></span>
<span data-ttu-id="77892-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77892-129">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77892-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77892-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="77892-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77892-131">Request</span></span>
<span data-ttu-id="77892-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77892-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="77892-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="77892-133">Response</span></span>
<span data-ttu-id="77892-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77892-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




