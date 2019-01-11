---
title: Abrufen von „managedAppPolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: de7f194aa6d8d47fe9944a08689d2b5bb9e83cf8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886450"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="dee38-103">Abrufen von „managedAppPolicy“</span><span class="sxs-lookup"><span data-stu-id="dee38-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="dee38-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dee38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dee38-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dee38-105">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dee38-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dee38-106">Prerequisites</span></span>
<span data-ttu-id="dee38-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dee38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dee38-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dee38-109">Permission type</span></span>|<span data-ttu-id="dee38-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dee38-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dee38-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dee38-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dee38-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dee38-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dee38-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dee38-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dee38-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dee38-114">Not supported.</span></span>|
|<span data-ttu-id="dee38-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dee38-115">Application</span></span>|<span data-ttu-id="dee38-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dee38-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dee38-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dee38-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dee38-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dee38-118">Optional query parameters</span></span>
<span data-ttu-id="dee38-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dee38-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dee38-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dee38-120">Request headers</span></span>
|<span data-ttu-id="dee38-121">Header</span><span class="sxs-lookup"><span data-stu-id="dee38-121">Header</span></span>|<span data-ttu-id="dee38-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dee38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dee38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dee38-123">Authorization</span></span>|<span data-ttu-id="dee38-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dee38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dee38-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dee38-125">Accept</span></span>|<span data-ttu-id="dee38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dee38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dee38-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dee38-127">Request body</span></span>
<span data-ttu-id="dee38-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dee38-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dee38-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dee38-129">Response</span></span>
<span data-ttu-id="dee38-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dee38-130">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dee38-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dee38-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dee38-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dee38-132">Request</span></span>
<span data-ttu-id="dee38-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dee38-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="dee38-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dee38-134">Response</span></span>
<span data-ttu-id="dee38-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dee38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



