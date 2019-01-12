---
title: Abrufen von „managedAppOperation“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43fa39cb4da9cf8468c0f0382cc614ac69006753
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963360"
---
# <a name="get-managedappoperation"></a><span data-ttu-id="9e717-103">Abrufen von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="9e717-103">Get managedAppOperation</span></span>

> <span data-ttu-id="9e717-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9e717-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e717-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9e717-105">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e717-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9e717-106">Prerequisites</span></span>
<span data-ttu-id="9e717-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e717-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e717-109">Permission type</span></span>|<span data-ttu-id="9e717-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e717-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e717-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e717-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e717-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e717-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9e717-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e717-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e717-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e717-114">Not supported.</span></span>|
|<span data-ttu-id="9e717-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e717-115">Application</span></span>|<span data-ttu-id="9e717-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e717-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e717-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e717-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e717-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9e717-118">Optional query parameters</span></span>
<span data-ttu-id="9e717-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9e717-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9e717-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e717-120">Request headers</span></span>
|<span data-ttu-id="9e717-121">Header</span><span class="sxs-lookup"><span data-stu-id="9e717-121">Header</span></span>|<span data-ttu-id="9e717-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9e717-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e717-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e717-123">Authorization</span></span>|<span data-ttu-id="9e717-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9e717-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e717-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9e717-125">Accept</span></span>|<span data-ttu-id="9e717-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e717-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e717-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e717-127">Request body</span></span>
<span data-ttu-id="9e717-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9e717-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e717-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e717-129">Response</span></span>
<span data-ttu-id="9e717-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9e717-130">If successful, this method returns a `200 OK` response code and [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e717-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e717-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e717-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e717-132">Request</span></span>
<span data-ttu-id="9e717-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e717-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

### <a name="response"></a><span data-ttu-id="9e717-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e717-134">Response</span></span>
<span data-ttu-id="9e717-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e717-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppOperation",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "State value",
    "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
    "version": "Version value"
  }
}
```



