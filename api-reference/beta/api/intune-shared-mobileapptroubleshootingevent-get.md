---
title: Abrufen von mobileAppTroubleshootingEvent
description: Beschreibt die MobileAppTroubleshootingEvent Get-Methode, die Microsoft Graph-API für Intune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6d151c28e909aecc1a0f20775d75813e0666df71
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429921"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="3d2b9-103">Abrufen von mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3d2b9-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="3d2b9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d2b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d2b9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d2b9-107">Lesen Sie Eigenschaften und Beziehungen des [MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d2b9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d2b9-108">Prerequisites</span></span>
<span data-ttu-id="3d2b9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d2b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d2b9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d2b9-111">Permission type</span></span>|<span data-ttu-id="3d2b9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d2b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d2b9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d2b9-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="3d2b9-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="3d2b9-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="3d2b9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d2b9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3d2b9-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="3d2b9-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="3d2b9-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d2b9-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3d2b9-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d2b9-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d2b9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d2b9-119">Not supported.</span></span>|
|<span data-ttu-id="3d2b9-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d2b9-120">Application</span></span>|<span data-ttu-id="3d2b9-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d2b9-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d2b9-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d2b9-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d2b9-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3d2b9-123">Optional query parameters</span></span>
<span data-ttu-id="3d2b9-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-124">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d2b9-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d2b9-125">Request headers</span></span>
|<span data-ttu-id="3d2b9-126">Header</span><span class="sxs-lookup"><span data-stu-id="3d2b9-126">Header</span></span>|<span data-ttu-id="3d2b9-127">Wert</span><span class="sxs-lookup"><span data-stu-id="3d2b9-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d2b9-128">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3d2b9-128">Authorization</span></span>|<span data-ttu-id="3d2b9-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d2b9-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d2b9-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3d2b9-130">Accept</span></span>|<span data-ttu-id="3d2b9-131">application/json</span><span class="sxs-lookup"><span data-stu-id="3d2b9-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d2b9-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d2b9-132">Request body</span></span>
<span data-ttu-id="3d2b9-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d2b9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d2b9-134">Response</span></span>
<span data-ttu-id="3d2b9-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-135">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d2b9-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d2b9-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d2b9-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d2b9-137">Request</span></span>
<span data-ttu-id="3d2b9-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="3d2b9-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d2b9-139">Response</span></span>
<span data-ttu-id="3d2b9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d2b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
    "id": "77943c10-3c10-7794-103c-9477103c9477"
  }
}
```




