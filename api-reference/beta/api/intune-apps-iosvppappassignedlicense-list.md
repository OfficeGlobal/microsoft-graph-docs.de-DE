---
title: Liste iosVppAppAssignedLicenses
description: Listeneigenschaften und Beziehungen der IosVppAppAssignedLicense-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d8ab94aa7d5a20253792079604b0a9164544104
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966153"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="fbbeb-103">Liste iosVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="fbbeb-103">List iosVppAppAssignedLicenses</span></span>

> <span data-ttu-id="fbbeb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fbbeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbbeb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fbbeb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbbeb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fbbeb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbbeb-107">Listeneigenschaften und Beziehungen der [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="fbbeb-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbbeb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fbbeb-108">Prerequisites</span></span>
<span data-ttu-id="fbbeb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbbeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbbeb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fbbeb-111">Permission type</span></span>|<span data-ttu-id="fbbeb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fbbeb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbbeb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fbbeb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbbeb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbbeb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fbbeb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fbbeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbbeb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbbeb-116">Not supported.</span></span>|
|<span data-ttu-id="fbbeb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fbbeb-117">Application</span></span>|<span data-ttu-id="fbbeb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbbeb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbbeb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbbeb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="fbbeb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fbbeb-120">Request headers</span></span>
|<span data-ttu-id="fbbeb-121">Header</span><span class="sxs-lookup"><span data-stu-id="fbbeb-121">Header</span></span>|<span data-ttu-id="fbbeb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fbbeb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbbeb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbbeb-123">Authorization</span></span>|<span data-ttu-id="fbbeb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fbbeb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbbeb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fbbeb-125">Accept</span></span>|<span data-ttu-id="fbbeb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbbeb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbbeb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fbbeb-127">Request body</span></span>
<span data-ttu-id="fbbeb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fbbeb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbbeb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbbeb-129">Response</span></span>
<span data-ttu-id="fbbeb-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="fbbeb-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbbeb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fbbeb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbbeb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbbeb-132">Request</span></span>
<span data-ttu-id="fbbeb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fbbeb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="fbbeb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbbeb-134">Response</span></span>
<span data-ttu-id="fbbeb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbbeb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





