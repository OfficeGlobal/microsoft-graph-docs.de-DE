---
title: Liste mobileAppTroubleshootingEvents
description: Listeneigenschaften und Beziehungen der MobileAppTroubleshootingEvent-Objekte.
author: tfitzmac
ms.openlocfilehash: cee6872731977fedddced00f3bad678d3b3e42da
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308673"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="8c7fb-103">Liste mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="8c7fb-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="8c7fb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c7fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c7fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c7fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c7fb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c7fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c7fb-107">Listeneigenschaften und Beziehungen der [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="8c7fb-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c7fb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c7fb-108">Prerequisites</span></span>
<span data-ttu-id="8c7fb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c7fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c7fb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c7fb-111">Permission type</span></span>|<span data-ttu-id="8c7fb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c7fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c7fb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c7fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c7fb-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c7fb-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8c7fb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c7fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c7fb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c7fb-116">Not supported.</span></span>|
|<span data-ttu-id="8c7fb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c7fb-117">Application</span></span>|<span data-ttu-id="8c7fb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c7fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c7fb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c7fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8c7fb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c7fb-120">Request headers</span></span>
|<span data-ttu-id="8c7fb-121">Header</span><span class="sxs-lookup"><span data-stu-id="8c7fb-121">Header</span></span>|<span data-ttu-id="8c7fb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8c7fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c7fb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8c7fb-123">Authorization</span></span>|<span data-ttu-id="8c7fb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c7fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c7fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c7fb-125">Accept</span></span>|<span data-ttu-id="8c7fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c7fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c7fb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c7fb-127">Request body</span></span>
<span data-ttu-id="8c7fb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8c7fb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c7fb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c7fb-129">Response</span></span>
<span data-ttu-id="8c7fb-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="8c7fb-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c7fb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c7fb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c7fb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c7fb-132">Request</span></span>
<span data-ttu-id="8c7fb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c7fb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="8c7fb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c7fb-134">Response</span></span>
<span data-ttu-id="8c7fb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c7fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 623

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "applicationId": "Application Id value",
      "history": [
        {
          "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
          "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
        }
      ]
    }
  ]
}
```





