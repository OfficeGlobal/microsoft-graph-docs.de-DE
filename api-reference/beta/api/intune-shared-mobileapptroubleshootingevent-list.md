---
title: MobileAppTroubleshootingEvents aufListen
description: Beschreibt die mobileAppTroubleshootingEvent-Methode der Microsoft Graph-API für InTune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d34d37324e61e967b01b46e2a1ba842688862281
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976869"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="1c719-103">MobileAppTroubleshootingEvents aufListen</span><span class="sxs-lookup"><span data-stu-id="1c719-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="1c719-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="1c719-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1c719-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c719-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c719-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1c719-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c719-107">AufListen von Eigenschaften und Beziehungen der [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="1c719-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c719-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c719-108">Prerequisites</span></span>
<span data-ttu-id="1c719-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c719-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c719-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c719-111">Permission type</span></span>|<span data-ttu-id="1c719-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c719-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c719-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c719-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="1c719-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="1c719-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="1c719-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c719-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1c719-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="1c719-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="1c719-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c719-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1c719-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c719-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c719-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c719-119">Not supported.</span></span>|
|<span data-ttu-id="1c719-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c719-120">Application</span></span>|<span data-ttu-id="1c719-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c719-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c719-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c719-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="1c719-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c719-123">Request headers</span></span>
|<span data-ttu-id="1c719-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c719-124">Header</span></span>|<span data-ttu-id="1c719-125">Wert</span><span class="sxs-lookup"><span data-stu-id="1c719-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c719-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c719-126">Authorization</span></span>|<span data-ttu-id="1c719-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c719-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c719-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1c719-128">Accept</span></span>|<span data-ttu-id="1c719-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1c719-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c719-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c719-130">Request body</span></span>
<span data-ttu-id="1c719-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c719-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c719-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c719-132">Response</span></span>
<span data-ttu-id="1c719-133">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1c719-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c719-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c719-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c719-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c719-135">Request</span></span>
<span data-ttu-id="1c719-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c719-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="1c719-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c719-137">Response</span></span>
<span data-ttu-id="1c719-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c719-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477"
    }
  ]
}
```




