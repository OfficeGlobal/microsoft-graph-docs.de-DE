---
title: Abrufen von „managedAppConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7638112219202d6a76e10691b31092bdc065c32e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837058"
---
# <a name="get-managedappconfiguration"></a><span data-ttu-id="51516-103">Abrufen von „managedAppConfiguration“</span><span class="sxs-lookup"><span data-stu-id="51516-103">Get managedAppConfiguration</span></span>

> <span data-ttu-id="51516-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51516-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51516-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51516-105">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51516-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="51516-106">Prerequisites</span></span>
<span data-ttu-id="51516-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51516-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51516-109">Permission type</span></span>|<span data-ttu-id="51516-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51516-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51516-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51516-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51516-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51516-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="51516-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51516-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51516-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51516-114">Not supported.</span></span>|
|<span data-ttu-id="51516-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51516-115">Application</span></span>|<span data-ttu-id="51516-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51516-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51516-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51516-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51516-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="51516-118">Optional query parameters</span></span>
<span data-ttu-id="51516-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51516-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51516-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51516-120">Request headers</span></span>
|<span data-ttu-id="51516-121">Header</span><span class="sxs-lookup"><span data-stu-id="51516-121">Header</span></span>|<span data-ttu-id="51516-122">Wert</span><span class="sxs-lookup"><span data-stu-id="51516-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51516-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51516-123">Authorization</span></span>|<span data-ttu-id="51516-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="51516-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51516-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="51516-125">Accept</span></span>|<span data-ttu-id="51516-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51516-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51516-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51516-127">Request body</span></span>
<span data-ttu-id="51516-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="51516-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51516-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="51516-129">Response</span></span>
<span data-ttu-id="51516-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="51516-130">If successful, this method returns a `200 OK` response code and [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51516-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51516-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="51516-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51516-132">Request</span></span>
<span data-ttu-id="51516-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51516-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="51516-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="51516-134">Response</span></span>
<span data-ttu-id="51516-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51516-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```



