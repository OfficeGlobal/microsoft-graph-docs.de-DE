---
title: Funktion getUserIdsWithFlaggedAppRegistration
description: Noch nicht dokumentiert
ms.openlocfilehash: 48505328c44b06a267ecae281adc533409001dea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063561"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="a1463-103">Funktion getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a1463-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="a1463-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a1463-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1463-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1463-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1463-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a1463-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1463-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a1463-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1463-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a1463-108">Prerequisites</span></span>
<span data-ttu-id="a1463-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1463-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1463-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1463-111">Permission type</span></span>|<span data-ttu-id="a1463-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1463-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1463-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1463-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1463-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1463-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1463-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1463-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1463-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1463-116">Not supported.</span></span>|
|<span data-ttu-id="a1463-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1463-117">Application</span></span>|<span data-ttu-id="a1463-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1463-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1463-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1463-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="a1463-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1463-120">Request headers</span></span>
|<span data-ttu-id="a1463-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a1463-121">Header</span></span>|<span data-ttu-id="a1463-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a1463-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1463-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1463-123">Authorization</span></span>|<span data-ttu-id="a1463-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a1463-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1463-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1463-125">Accept</span></span>|<span data-ttu-id="a1463-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1463-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1463-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1463-127">Request body</span></span>
<span data-ttu-id="a1463-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a1463-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1463-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1463-129">Response</span></span>
<span data-ttu-id="a1463-130">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a1463-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1463-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1463-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1463-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1463-132">Request</span></span>
<span data-ttu-id="a1463-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1463-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="a1463-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1463-134">Response</span></span>
<span data-ttu-id="a1463-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1463-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





