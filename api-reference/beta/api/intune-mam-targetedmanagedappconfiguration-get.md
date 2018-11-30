---
title: targetedManagedAppConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des targetedManagedAppConfiguration-Objekts.
ms.openlocfilehash: c61a80b1775d6fd01854e4b931432781618151d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060495"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="5b68e-103">targetedManagedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="5b68e-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="5b68e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b68e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b68e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b68e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b68e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5b68e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b68e-107">Lesen von Eigenschaften und Beziehungen des [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b68e-107">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b68e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b68e-108">Prerequisites</span></span>
<span data-ttu-id="5b68e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b68e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b68e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b68e-111">Permission type</span></span>|<span data-ttu-id="5b68e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b68e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b68e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b68e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b68e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b68e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5b68e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b68e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b68e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b68e-116">Not supported.</span></span>|
|<span data-ttu-id="5b68e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b68e-117">Application</span></span>|<span data-ttu-id="5b68e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b68e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b68e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b68e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b68e-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5b68e-120">Optional query parameters</span></span>
<span data-ttu-id="5b68e-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b68e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5b68e-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b68e-122">Request headers</span></span>
|<span data-ttu-id="5b68e-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b68e-123">Header</span></span>|<span data-ttu-id="5b68e-124">Wert</span><span class="sxs-lookup"><span data-stu-id="5b68e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b68e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b68e-125">Authorization</span></span>|<span data-ttu-id="5b68e-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b68e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b68e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5b68e-127">Accept</span></span>|<span data-ttu-id="5b68e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b68e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b68e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b68e-129">Request body</span></span>
<span data-ttu-id="5b68e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b68e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b68e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b68e-131">Response</span></span>
<span data-ttu-id="5b68e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b68e-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b68e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b68e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b68e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b68e-134">Request</span></span>
<span data-ttu-id="5b68e-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b68e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5b68e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b68e-136">Response</span></span>
<span data-ttu-id="5b68e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b68e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```




