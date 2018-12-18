---
title: Liste iosVppAppAssignedLicenses
description: Listeneigenschaften und Beziehungen der IosVppAppAssignedLicense-Objekte.
author: tfitzmac
ms.openlocfilehash: ee5787593a841246165ad10673a772b6e24ddf09
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358184"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="4e3ca-103">Liste iosVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="4e3ca-103">List iosVppAppAssignedLicenses</span></span>

> <span data-ttu-id="4e3ca-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e3ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e3ca-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e3ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e3ca-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4e3ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e3ca-107">Listeneigenschaften und Beziehungen der [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="4e3ca-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e3ca-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e3ca-108">Prerequisites</span></span>
<span data-ttu-id="4e3ca-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e3ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e3ca-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e3ca-111">Permission type</span></span>|<span data-ttu-id="4e3ca-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e3ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e3ca-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e3ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e3ca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e3ca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4e3ca-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e3ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e3ca-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e3ca-116">Not supported.</span></span>|
|<span data-ttu-id="4e3ca-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e3ca-117">Application</span></span>|<span data-ttu-id="4e3ca-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e3ca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e3ca-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e3ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="4e3ca-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e3ca-120">Request headers</span></span>
|<span data-ttu-id="4e3ca-121">Header</span><span class="sxs-lookup"><span data-stu-id="4e3ca-121">Header</span></span>|<span data-ttu-id="4e3ca-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4e3ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e3ca-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4e3ca-123">Authorization</span></span>|<span data-ttu-id="4e3ca-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4e3ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e3ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e3ca-125">Accept</span></span>|<span data-ttu-id="4e3ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e3ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e3ca-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e3ca-127">Request body</span></span>
<span data-ttu-id="4e3ca-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4e3ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e3ca-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e3ca-129">Response</span></span>
<span data-ttu-id="4e3ca-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="4e3ca-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e3ca-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e3ca-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e3ca-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e3ca-132">Request</span></span>
<span data-ttu-id="4e3ca-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e3ca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="4e3ca-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e3ca-134">Response</span></span>
<span data-ttu-id="4e3ca-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e3ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
      "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





