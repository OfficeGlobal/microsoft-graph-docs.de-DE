---
title: Liste remoteActionAudits
description: Listeneigenschaften und Beziehungen der RemoteActionAudit-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8124c5da95e01c1c0513e5f8ac88cd45d7943fd5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971172"
---
# <a name="list-remoteactionaudits"></a><span data-ttu-id="69878-103">Liste remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="69878-103">List remoteActionAudits</span></span>

> <span data-ttu-id="69878-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="69878-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69878-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69878-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69878-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69878-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69878-107">Listeneigenschaften und Beziehungen der [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="69878-107">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69878-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="69878-108">Prerequisites</span></span>
<span data-ttu-id="69878-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69878-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69878-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69878-111">Permission type</span></span>|<span data-ttu-id="69878-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69878-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69878-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69878-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69878-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="69878-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="69878-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69878-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69878-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69878-116">Not supported.</span></span>|
|<span data-ttu-id="69878-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69878-117">Application</span></span>|<span data-ttu-id="69878-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69878-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69878-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69878-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="69878-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69878-120">Request headers</span></span>
|<span data-ttu-id="69878-121">Header</span><span class="sxs-lookup"><span data-stu-id="69878-121">Header</span></span>|<span data-ttu-id="69878-122">Wert</span><span class="sxs-lookup"><span data-stu-id="69878-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69878-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69878-123">Authorization</span></span>|<span data-ttu-id="69878-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="69878-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69878-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="69878-125">Accept</span></span>|<span data-ttu-id="69878-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69878-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69878-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69878-127">Request body</span></span>
<span data-ttu-id="69878-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="69878-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69878-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="69878-129">Response</span></span>
<span data-ttu-id="69878-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="69878-130">If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69878-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69878-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="69878-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69878-132">Request</span></span>
<span data-ttu-id="69878-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69878-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
```

### <a name="response"></a><span data-ttu-id="69878-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="69878-134">Response</span></span>
<span data-ttu-id="69878-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69878-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteActionAudit",
      "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
      "action": "factoryReset",
      "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
      "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
      "deviceIMEI": "Device IMEI value",
      "actionState": "pending"
    }
  ]
}
```





