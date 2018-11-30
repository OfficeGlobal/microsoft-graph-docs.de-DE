---
title: Abrufen von embeddedSIMActivationCodePool
description: Lesen Sie Eigenschaften und Beziehungen des EmbeddedSIMActivationCodePool-Objekts.
ms.openlocfilehash: 97752212df207e5c530c785b699382ac8c0f4a64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059194"
---
# <a name="get-embeddedsimactivationcodepool"></a><span data-ttu-id="69f44-103">Abrufen von embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="69f44-103">Get embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="69f44-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="69f44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69f44-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69f44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69f44-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69f44-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69f44-107">Lesen Sie Eigenschaften und Beziehungen des [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="69f44-107">Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69f44-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="69f44-108">Prerequisites</span></span>
<span data-ttu-id="69f44-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f44-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69f44-111">Permission type</span></span>|<span data-ttu-id="69f44-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69f44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f44-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69f44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69f44-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69f44-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="69f44-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69f44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f44-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69f44-116">Not supported.</span></span>|
|<span data-ttu-id="69f44-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69f44-117">Application</span></span>|<span data-ttu-id="69f44-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69f44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f44-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69f44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69f44-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="69f44-120">Optional query parameters</span></span>
<span data-ttu-id="69f44-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="69f44-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="69f44-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69f44-122">Request headers</span></span>
|<span data-ttu-id="69f44-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="69f44-123">Header</span></span>|<span data-ttu-id="69f44-124">Wert</span><span class="sxs-lookup"><span data-stu-id="69f44-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f44-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f44-125">Authorization</span></span>|<span data-ttu-id="69f44-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="69f44-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f44-127">Accept</span><span class="sxs-lookup"><span data-stu-id="69f44-127">Accept</span></span>|<span data-ttu-id="69f44-128">application/json</span><span class="sxs-lookup"><span data-stu-id="69f44-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f44-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69f44-129">Request body</span></span>
<span data-ttu-id="69f44-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="69f44-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f44-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="69f44-131">Response</span></span>
<span data-ttu-id="69f44-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="69f44-132">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f44-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69f44-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="69f44-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69f44-134">Request</span></span>
<span data-ttu-id="69f44-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69f44-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

### <a name="response"></a><span data-ttu-id="69f44-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="69f44-136">Response</span></span>
<span data-ttu-id="69f44-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69f44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
    "id": "ec308741-8741-ec30-4187-30ec418730ec",
    "displayName": "Display Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "activationCodes": [
      {
        "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
        "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
        "matchingIdentifier": "Matching Identifier value",
        "smdpPlusServerAddress": "Smdp Plus Server Address value"
      }
    ],
    "activationCodeCount": 3
  }
}
```





