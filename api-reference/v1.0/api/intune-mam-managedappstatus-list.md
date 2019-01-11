---
title: Auflisten von „managedAppStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAppStatus auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b5a01f37045c7c9927604a87441ef6d5e007092c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855223"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="bf820-103">Auflisten von „managedAppStatus“</span><span class="sxs-lookup"><span data-stu-id="bf820-103">List managedAppStatuses</span></span>

> <span data-ttu-id="bf820-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bf820-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf820-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="bf820-105">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf820-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bf820-106">Prerequisites</span></span>
<span data-ttu-id="bf820-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf820-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf820-109">Permission type</span></span>|<span data-ttu-id="bf820-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf820-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf820-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf820-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bf820-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf820-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bf820-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf820-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf820-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf820-114">Not supported.</span></span>|
|<span data-ttu-id="bf820-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf820-115">Application</span></span>|<span data-ttu-id="bf820-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf820-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf820-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf820-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="bf820-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf820-118">Request headers</span></span>
|<span data-ttu-id="bf820-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bf820-119">Header</span></span>|<span data-ttu-id="bf820-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bf820-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf820-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf820-121">Authorization</span></span>|<span data-ttu-id="bf820-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bf820-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf820-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bf820-123">Accept</span></span>|<span data-ttu-id="bf820-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bf820-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf820-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf820-125">Request body</span></span>
<span data-ttu-id="bf820-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bf820-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf820-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf820-127">Response</span></span>
<span data-ttu-id="bf820-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bf820-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf820-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf820-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf820-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf820-130">Request</span></span>
<span data-ttu-id="bf820-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf820-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="bf820-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf820-132">Response</span></span>
<span data-ttu-id="bf820-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf820-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatus",
      "displayName": "Display Name value",
      "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
      "version": "Version value"
    }
  ]
}
```



