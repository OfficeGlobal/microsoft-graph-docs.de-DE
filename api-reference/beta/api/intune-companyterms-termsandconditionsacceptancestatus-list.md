---
title: Auflisten von „termsAndConditionsAcceptanceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditionsAcceptanceStatus auf.
ms.openlocfilehash: 0f519f399b1c13f227b0375270d45ca229c4081e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061190"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="faf3b-103">Auflisten von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="faf3b-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="faf3b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="faf3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faf3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="faf3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faf3b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="faf3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="faf3b-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="faf3b-107">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="faf3b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="faf3b-108">Prerequisites</span></span>
<span data-ttu-id="faf3b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faf3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf3b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="faf3b-111">Permission type</span></span>|<span data-ttu-id="faf3b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="faf3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faf3b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="faf3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="faf3b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="faf3b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="faf3b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="faf3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faf3b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="faf3b-116">Not supported.</span></span>|
|<span data-ttu-id="faf3b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="faf3b-117">Application</span></span>|<span data-ttu-id="faf3b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="faf3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faf3b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="faf3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="faf3b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="faf3b-120">Request headers</span></span>
|<span data-ttu-id="faf3b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="faf3b-121">Header</span></span>|<span data-ttu-id="faf3b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="faf3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faf3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="faf3b-123">Authorization</span></span>|<span data-ttu-id="faf3b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="faf3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faf3b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="faf3b-125">Accept</span></span>|<span data-ttu-id="faf3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="faf3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faf3b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="faf3b-127">Request body</span></span>
<span data-ttu-id="faf3b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="faf3b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faf3b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="faf3b-129">Response</span></span>
<span data-ttu-id="faf3b-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="faf3b-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faf3b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="faf3b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="faf3b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="faf3b-132">Request</span></span>
<span data-ttu-id="faf3b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="faf3b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="faf3b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="faf3b-134">Response</span></span>
<span data-ttu-id="faf3b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="faf3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
      "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
      "userDisplayName": "User Display Name value",
      "acceptedVersion": 15,
      "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
    }
  ]
}
```





