---
title: Auflisten von „termsAndConditions“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditions auf.
author: tfitzmac
ms.openlocfilehash: 5a5613484d25c84b5cb01e631d97e93280e5c060
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327552"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="f233a-103">Auflisten von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="f233a-103">List termsAndConditionses</span></span>

> <span data-ttu-id="f233a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f233a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f233a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f233a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f233a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f233a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f233a-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f233a-107">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f233a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f233a-108">Prerequisites</span></span>
<span data-ttu-id="f233a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f233a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f233a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f233a-111">Permission type</span></span>|<span data-ttu-id="f233a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f233a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f233a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f233a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f233a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f233a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f233a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f233a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f233a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f233a-116">Not supported.</span></span>|
|<span data-ttu-id="f233a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f233a-117">Application</span></span>|<span data-ttu-id="f233a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f233a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f233a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f233a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="f233a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f233a-120">Request headers</span></span>
|<span data-ttu-id="f233a-121">Header</span><span class="sxs-lookup"><span data-stu-id="f233a-121">Header</span></span>|<span data-ttu-id="f233a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f233a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f233a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f233a-123">Authorization</span></span>|<span data-ttu-id="f233a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f233a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f233a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f233a-125">Accept</span></span>|<span data-ttu-id="f233a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f233a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f233a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f233a-127">Request body</span></span>
<span data-ttu-id="f233a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f233a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f233a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f233a-129">Response</span></span>
<span data-ttu-id="f233a-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f233a-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f233a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f233a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f233a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f233a-132">Request</span></span>
<span data-ttu-id="f233a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f233a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="f233a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f233a-134">Response</span></span>
<span data-ttu-id="f233a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f233a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```





