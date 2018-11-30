---
title: Auflisten von „mobileAppCategory“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs mobileAppCategory auf.
ms.openlocfilehash: bc39e2653bab4840fedc390ce6cb7497bcfd9606
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065168"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="0a724-103">Auflisten von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="0a724-103">List mobileAppCategories</span></span>

> <span data-ttu-id="0a724-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0a724-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a724-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a724-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a724-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0a724-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a724-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) auf.</span><span class="sxs-lookup"><span data-stu-id="0a724-107">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a724-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0a724-108">Prerequisites</span></span>
<span data-ttu-id="0a724-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a724-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a724-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a724-111">Permission type</span></span>|<span data-ttu-id="0a724-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a724-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a724-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a724-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a724-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a724-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0a724-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a724-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a724-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a724-116">Not supported.</span></span>|
|<span data-ttu-id="0a724-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a724-117">Application</span></span>|<span data-ttu-id="0a724-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a724-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a724-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a724-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="0a724-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a724-120">Request headers</span></span>
|<span data-ttu-id="0a724-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0a724-121">Header</span></span>|<span data-ttu-id="0a724-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0a724-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a724-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a724-123">Authorization</span></span>|<span data-ttu-id="0a724-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a724-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a724-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a724-125">Accept</span></span>|<span data-ttu-id="0a724-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a724-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a724-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a724-127">Request body</span></span>
<span data-ttu-id="0a724-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0a724-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a724-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a724-129">Response</span></span>
<span data-ttu-id="0a724-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0a724-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a724-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a724-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a724-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a724-132">Request</span></span>
<span data-ttu-id="0a724-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a724-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="0a724-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a724-134">Response</span></span>
<span data-ttu-id="0a724-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a724-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppCategory",
      "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





