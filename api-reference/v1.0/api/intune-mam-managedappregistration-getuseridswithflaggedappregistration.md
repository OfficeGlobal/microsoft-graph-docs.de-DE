---
title: Funktion getUserIdsWithFlaggedAppRegistration
description: Noch nicht dokumentiert
ms.openlocfilehash: a33f59c1dab1cbdfb34dd62924d8724e71ac2e7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017380"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="b78b9-103">Funktion getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="b78b9-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="b78b9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b78b9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b78b9-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b78b9-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b78b9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b78b9-106">Prerequisites</span></span>
<span data-ttu-id="b78b9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b78b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b78b9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b78b9-109">Permission type</span></span>|<span data-ttu-id="b78b9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b78b9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b78b9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b78b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b78b9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b78b9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b78b9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b78b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b78b9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b78b9-114">Not supported.</span></span>|
|<span data-ttu-id="b78b9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b78b9-115">Application</span></span>|<span data-ttu-id="b78b9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b78b9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b78b9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b78b9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="b78b9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b78b9-118">Request headers</span></span>
|<span data-ttu-id="b78b9-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b78b9-119">Header</span></span>|<span data-ttu-id="b78b9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b78b9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b78b9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b78b9-121">Authorization</span></span>|<span data-ttu-id="b78b9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b78b9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b78b9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b78b9-123">Accept</span></span>|<span data-ttu-id="b78b9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b78b9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b78b9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b78b9-125">Request body</span></span>
<span data-ttu-id="b78b9-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b78b9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b78b9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b78b9-127">Response</span></span>
<span data-ttu-id="b78b9-128">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b78b9-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b78b9-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b78b9-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b78b9-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b78b9-130">Request</span></span>
<span data-ttu-id="b78b9-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b78b9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="b78b9-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b78b9-132">Response</span></span>
<span data-ttu-id="b78b9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b78b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```


