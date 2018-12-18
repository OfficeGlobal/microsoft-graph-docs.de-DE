---
title: Liste iosVppAppAssignedUserLicenses
description: Listeneigenschaften und Beziehungen der IosVppAppAssignedUserLicense-Objekte.
author: tfitzmac
ms.openlocfilehash: 4e4de201d570813a3b985430d97774444d1e76f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302492"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="acdfd-103">Liste iosVppAppAssignedUserLicenses</span><span class="sxs-lookup"><span data-stu-id="acdfd-103">List iosVppAppAssignedUserLicenses</span></span>

> <span data-ttu-id="acdfd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="acdfd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acdfd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acdfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acdfd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acdfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acdfd-107">Listeneigenschaften und Beziehungen der [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="acdfd-107">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acdfd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="acdfd-108">Prerequisites</span></span>
<span data-ttu-id="acdfd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acdfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acdfd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acdfd-111">Permission type</span></span>|<span data-ttu-id="acdfd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acdfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acdfd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acdfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acdfd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="acdfd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="acdfd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acdfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acdfd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acdfd-116">Not supported.</span></span>|
|<span data-ttu-id="acdfd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acdfd-117">Application</span></span>|<span data-ttu-id="acdfd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acdfd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acdfd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acdfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="acdfd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acdfd-120">Request headers</span></span>
|<span data-ttu-id="acdfd-121">Header</span><span class="sxs-lookup"><span data-stu-id="acdfd-121">Header</span></span>|<span data-ttu-id="acdfd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="acdfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acdfd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="acdfd-123">Authorization</span></span>|<span data-ttu-id="acdfd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="acdfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acdfd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="acdfd-125">Accept</span></span>|<span data-ttu-id="acdfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acdfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acdfd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acdfd-127">Request body</span></span>
<span data-ttu-id="acdfd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="acdfd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acdfd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="acdfd-129">Response</span></span>
<span data-ttu-id="acdfd-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="acdfd-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acdfd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acdfd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="acdfd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acdfd-132">Request</span></span>
<span data-ttu-id="acdfd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acdfd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="acdfd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="acdfd-134">Response</span></span>
<span data-ttu-id="acdfd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acdfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





