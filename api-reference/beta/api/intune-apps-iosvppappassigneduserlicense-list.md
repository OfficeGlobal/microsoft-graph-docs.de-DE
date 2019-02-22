---
title: IosVppAppAssignedUserLicenses aufListen
description: AufListen von Eigenschaften und Beziehungen der iosVppAppAssignedUserLicense-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17bea16e6ae3916950ea3d107e41291daf081e45
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155027"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="19a8e-103">IosVppAppAssignedUserLicenses aufListen</span><span class="sxs-lookup"><span data-stu-id="19a8e-103">List iosVppAppAssignedUserLicenses</span></span>

> <span data-ttu-id="19a8e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19a8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19a8e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="19a8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19a8e-106">AufListen von Eigenschaften und Beziehungen der [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="19a8e-106">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19a8e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="19a8e-107">Prerequisites</span></span>
<span data-ttu-id="19a8e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19a8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19a8e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19a8e-110">Permission type</span></span>|<span data-ttu-id="19a8e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19a8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19a8e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19a8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19a8e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="19a8e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="19a8e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19a8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19a8e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19a8e-115">Not supported.</span></span>|
|<span data-ttu-id="19a8e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19a8e-116">Application</span></span>|<span data-ttu-id="19a8e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19a8e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19a8e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19a8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="19a8e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19a8e-119">Request headers</span></span>
|<span data-ttu-id="19a8e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="19a8e-120">Header</span></span>|<span data-ttu-id="19a8e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="19a8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19a8e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a8e-122">Authorization</span></span>|<span data-ttu-id="19a8e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="19a8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19a8e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="19a8e-124">Accept</span></span>|<span data-ttu-id="19a8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19a8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19a8e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19a8e-126">Request body</span></span>
<span data-ttu-id="19a8e-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="19a8e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19a8e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="19a8e-128">Response</span></span>
<span data-ttu-id="19a8e-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="19a8e-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19a8e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19a8e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="19a8e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19a8e-131">Request</span></span>
<span data-ttu-id="19a8e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19a8e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="19a8e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="19a8e-133">Response</span></span>
<span data-ttu-id="19a8e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19a8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




