---
title: Abrufen von „managedAppPolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 439a301b1693f49c82c17654c98489fbaa243f48
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960329"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="b0e37-103">Abrufen von „managedAppPolicy“</span><span class="sxs-lookup"><span data-stu-id="b0e37-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="b0e37-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b0e37-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0e37-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e37-105">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0e37-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b0e37-106">Prerequisites</span></span>
<span data-ttu-id="b0e37-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0e37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0e37-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0e37-109">Permission type</span></span>|<span data-ttu-id="b0e37-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0e37-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0e37-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0e37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0e37-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0e37-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b0e37-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0e37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0e37-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0e37-114">Not supported.</span></span>|
|<span data-ttu-id="b0e37-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0e37-115">Application</span></span>|<span data-ttu-id="b0e37-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0e37-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0e37-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0e37-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0e37-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b0e37-118">Optional query parameters</span></span>
<span data-ttu-id="b0e37-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b0e37-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b0e37-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0e37-120">Request headers</span></span>
|<span data-ttu-id="b0e37-121">Header</span><span class="sxs-lookup"><span data-stu-id="b0e37-121">Header</span></span>|<span data-ttu-id="b0e37-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b0e37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0e37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0e37-123">Authorization</span></span>|<span data-ttu-id="b0e37-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b0e37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0e37-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b0e37-125">Accept</span></span>|<span data-ttu-id="b0e37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0e37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0e37-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0e37-127">Request body</span></span>
<span data-ttu-id="b0e37-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b0e37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0e37-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0e37-129">Response</span></span>
<span data-ttu-id="b0e37-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b0e37-130">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0e37-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0e37-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0e37-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0e37-132">Request</span></span>
<span data-ttu-id="b0e37-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b0e37-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="b0e37-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0e37-134">Response</span></span>
<span data-ttu-id="b0e37-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0e37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
    "version": "Version value"
  }
}
```



