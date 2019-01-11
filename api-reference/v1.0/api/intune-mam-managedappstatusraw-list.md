---
title: Auflisten von „managedAppStatusRaw“
description: Auflisten von Eigenschaften und Beziehungen der managedAppStatusRaw-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7dd30f4731042307f543bde7420795b95bc496bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828798"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="21e49-103">Auflisten von „managedAppStatusRaw“</span><span class="sxs-lookup"><span data-stu-id="21e49-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="21e49-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21e49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21e49-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) auf.</span><span class="sxs-lookup"><span data-stu-id="21e49-105">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21e49-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21e49-106">Prerequisites</span></span>
<span data-ttu-id="21e49-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21e49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21e49-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21e49-109">Permission type</span></span>|<span data-ttu-id="21e49-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21e49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21e49-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21e49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21e49-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21e49-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="21e49-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21e49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21e49-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21e49-114">Not supported.</span></span>|
|<span data-ttu-id="21e49-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21e49-115">Application</span></span>|<span data-ttu-id="21e49-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21e49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21e49-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21e49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="21e49-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21e49-118">Request headers</span></span>
|<span data-ttu-id="21e49-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="21e49-119">Header</span></span>|<span data-ttu-id="21e49-120">Wert</span><span class="sxs-lookup"><span data-stu-id="21e49-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21e49-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="21e49-121">Authorization</span></span>|<span data-ttu-id="21e49-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21e49-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21e49-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21e49-123">Accept</span></span>|<span data-ttu-id="21e49-124">application/json</span><span class="sxs-lookup"><span data-stu-id="21e49-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21e49-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21e49-125">Request body</span></span>
<span data-ttu-id="21e49-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="21e49-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21e49-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="21e49-127">Response</span></span>
<span data-ttu-id="21e49-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21e49-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21e49-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21e49-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="21e49-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21e49-130">Request</span></span>
<span data-ttu-id="21e49-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21e49-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="21e49-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="21e49-132">Response</span></span>
<span data-ttu-id="21e49-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21e49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatusRaw",
      "displayName": "Display Name value",
      "id": "80847581-7581-8084-8175-848081758480",
      "version": "Version value",
      "content": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```



