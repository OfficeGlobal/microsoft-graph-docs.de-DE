---
title: Abrufen von remoteActionAudit
description: Lesen Sie Eigenschaften und Beziehungen des RemoteActionAudit-Objekts.
author: tfitzmac
ms.openlocfilehash: d5400eefe34419a725681d8870bfae513d192237
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349539"
---
# <a name="get-remoteactionaudit"></a><span data-ttu-id="4293c-103">Abrufen von remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4293c-103">Get remoteActionAudit</span></span>

> <span data-ttu-id="4293c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4293c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4293c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4293c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4293c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4293c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4293c-107">Lesen Sie Eigenschaften und Beziehungen des [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4293c-107">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4293c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4293c-108">Prerequisites</span></span>
<span data-ttu-id="4293c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4293c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4293c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4293c-111">Permission type</span></span>|<span data-ttu-id="4293c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4293c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4293c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4293c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4293c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4293c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4293c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4293c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4293c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4293c-116">Not supported.</span></span>|
|<span data-ttu-id="4293c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4293c-117">Application</span></span>|<span data-ttu-id="4293c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4293c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4293c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4293c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4293c-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4293c-120">Optional query parameters</span></span>
<span data-ttu-id="4293c-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4293c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4293c-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4293c-122">Request headers</span></span>
|<span data-ttu-id="4293c-123">Header</span><span class="sxs-lookup"><span data-stu-id="4293c-123">Header</span></span>|<span data-ttu-id="4293c-124">Wert</span><span class="sxs-lookup"><span data-stu-id="4293c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4293c-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4293c-125">Authorization</span></span>|<span data-ttu-id="4293c-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4293c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4293c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4293c-127">Accept</span></span>|<span data-ttu-id="4293c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4293c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4293c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4293c-129">Request body</span></span>
<span data-ttu-id="4293c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4293c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4293c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="4293c-131">Response</span></span>
<span data-ttu-id="4293c-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4293c-132">If successful, this method returns a `200 OK` response code and [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4293c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4293c-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4293c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4293c-134">Request</span></span>
<span data-ttu-id="4293c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4293c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### <a name="response"></a><span data-ttu-id="4293c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4293c-136">Response</span></span>
<span data-ttu-id="4293c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4293c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "value": {
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
}
```





