---
title: Abrufen von „managedAppConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 78c174d2e9ae525d6ef6d2cda116501b831dd44c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965467"
---
# <a name="get-managedappconfiguration"></a><span data-ttu-id="a098f-103">Abrufen von „managedAppConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a098f-103">Get managedAppConfiguration</span></span>

> <span data-ttu-id="a098f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a098f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a098f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a098f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a098f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a098f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a098f-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a098f-107">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a098f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a098f-108">Prerequisites</span></span>
<span data-ttu-id="a098f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a098f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a098f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a098f-111">Permission type</span></span>|<span data-ttu-id="a098f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a098f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a098f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a098f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a098f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a098f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a098f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a098f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a098f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a098f-116">Not supported.</span></span>|
|<span data-ttu-id="a098f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a098f-117">Application</span></span>|<span data-ttu-id="a098f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a098f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a098f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a098f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a098f-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a098f-120">Optional query parameters</span></span>
<span data-ttu-id="a098f-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a098f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a098f-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a098f-122">Request headers</span></span>
|<span data-ttu-id="a098f-123">Header</span><span class="sxs-lookup"><span data-stu-id="a098f-123">Header</span></span>|<span data-ttu-id="a098f-124">Wert</span><span class="sxs-lookup"><span data-stu-id="a098f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a098f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a098f-125">Authorization</span></span>|<span data-ttu-id="a098f-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a098f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a098f-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a098f-127">Accept</span></span>|<span data-ttu-id="a098f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a098f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a098f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a098f-129">Request body</span></span>
<span data-ttu-id="a098f-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a098f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a098f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a098f-131">Response</span></span>
<span data-ttu-id="a098f-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a098f-132">If successful, this method returns a `200 OK` response code and [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a098f-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a098f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a098f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a098f-134">Request</span></span>
<span data-ttu-id="a098f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a098f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="a098f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a098f-136">Response</span></span>
<span data-ttu-id="a098f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a098f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





