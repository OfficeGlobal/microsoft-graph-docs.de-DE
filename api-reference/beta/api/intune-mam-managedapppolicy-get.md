---
title: Abrufen von „managedAppPolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicy.
ms.openlocfilehash: 04daf977169d2e0c28ac034fc95807877d2d495c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061071"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="63e47-103">Abrufen von „managedAppPolicy“</span><span class="sxs-lookup"><span data-stu-id="63e47-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="63e47-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="63e47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63e47-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="63e47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63e47-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="63e47-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63e47-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63e47-107">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63e47-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="63e47-108">Prerequisites</span></span>
<span data-ttu-id="63e47-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63e47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63e47-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63e47-111">Permission type</span></span>|<span data-ttu-id="63e47-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63e47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63e47-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63e47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63e47-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="63e47-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="63e47-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63e47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63e47-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63e47-116">Not supported.</span></span>|
|<span data-ttu-id="63e47-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63e47-117">Application</span></span>|<span data-ttu-id="63e47-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63e47-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63e47-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63e47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63e47-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="63e47-120">Optional query parameters</span></span>
<span data-ttu-id="63e47-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="63e47-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="63e47-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63e47-122">Request headers</span></span>
|<span data-ttu-id="63e47-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="63e47-123">Header</span></span>|<span data-ttu-id="63e47-124">Wert</span><span class="sxs-lookup"><span data-stu-id="63e47-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63e47-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="63e47-125">Authorization</span></span>|<span data-ttu-id="63e47-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="63e47-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63e47-127">Accept</span><span class="sxs-lookup"><span data-stu-id="63e47-127">Accept</span></span>|<span data-ttu-id="63e47-128">application/json</span><span class="sxs-lookup"><span data-stu-id="63e47-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63e47-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63e47-129">Request body</span></span>
<span data-ttu-id="63e47-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="63e47-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63e47-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="63e47-131">Response</span></span>
<span data-ttu-id="63e47-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="63e47-132">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63e47-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63e47-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="63e47-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63e47-134">Request</span></span>
<span data-ttu-id="63e47-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63e47-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="63e47-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="63e47-136">Response</span></span>
<span data-ttu-id="63e47-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63e47-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





