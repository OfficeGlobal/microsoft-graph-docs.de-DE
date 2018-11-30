---
title: Liste iosVppAppAssignedUserLicenses
description: Listeneigenschaften und Beziehungen der IosVppAppAssignedUserLicense-Objekte.
ms.openlocfilehash: 7ab7b55dfdcd9f8cbe2d015f46ac013e7840db26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064537"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="da1fb-103">Liste iosVppAppAssignedUserLicenses</span><span class="sxs-lookup"><span data-stu-id="da1fb-103">List iosVppAppAssignedUserLicenses</span></span>

> <span data-ttu-id="da1fb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="da1fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da1fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da1fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da1fb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="da1fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da1fb-107">Listeneigenschaften und Beziehungen der [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="da1fb-107">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da1fb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da1fb-108">Prerequisites</span></span>
<span data-ttu-id="da1fb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da1fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da1fb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da1fb-111">Permission type</span></span>|<span data-ttu-id="da1fb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da1fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da1fb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da1fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da1fb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da1fb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da1fb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da1fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da1fb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da1fb-116">Not supported.</span></span>|
|<span data-ttu-id="da1fb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da1fb-117">Application</span></span>|<span data-ttu-id="da1fb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da1fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da1fb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da1fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="da1fb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da1fb-120">Request headers</span></span>
|<span data-ttu-id="da1fb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="da1fb-121">Header</span></span>|<span data-ttu-id="da1fb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="da1fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da1fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da1fb-123">Authorization</span></span>|<span data-ttu-id="da1fb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da1fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da1fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da1fb-125">Accept</span></span>|<span data-ttu-id="da1fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da1fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da1fb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da1fb-127">Request body</span></span>
<span data-ttu-id="da1fb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="da1fb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da1fb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="da1fb-129">Response</span></span>
<span data-ttu-id="da1fb-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="da1fb-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da1fb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da1fb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="da1fb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da1fb-132">Request</span></span>
<span data-ttu-id="da1fb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da1fb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="da1fb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="da1fb-134">Response</span></span>
<span data-ttu-id="da1fb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da1fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
      "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





