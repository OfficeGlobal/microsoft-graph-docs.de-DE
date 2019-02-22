---
title: IosVppAppAssignedLicenses aufListen
description: AufListen von Eigenschaften und Beziehungen der iosVppAppAssignedLicense-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc15b7c9dd13785e74f6d55fb70dc451bb227de7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148895"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="84958-103">IosVppAppAssignedLicenses aufListen</span><span class="sxs-lookup"><span data-stu-id="84958-103">List iosVppAppAssignedLicenses</span></span>

> <span data-ttu-id="84958-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84958-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84958-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="84958-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84958-106">AufListen von Eigenschaften und Beziehungen der [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="84958-106">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84958-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84958-107">Prerequisites</span></span>
<span data-ttu-id="84958-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84958-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84958-110">Permission type</span></span>|<span data-ttu-id="84958-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84958-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84958-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84958-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84958-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84958-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84958-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84958-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84958-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84958-115">Not supported.</span></span>|
|<span data-ttu-id="84958-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84958-116">Application</span></span>|<span data-ttu-id="84958-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84958-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84958-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84958-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="84958-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84958-119">Request headers</span></span>
|<span data-ttu-id="84958-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="84958-120">Header</span></span>|<span data-ttu-id="84958-121">Wert</span><span class="sxs-lookup"><span data-stu-id="84958-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84958-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84958-122">Authorization</span></span>|<span data-ttu-id="84958-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84958-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84958-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84958-124">Accept</span></span>|<span data-ttu-id="84958-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84958-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84958-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84958-126">Request body</span></span>
<span data-ttu-id="84958-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="84958-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84958-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="84958-128">Response</span></span>
<span data-ttu-id="84958-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="84958-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84958-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84958-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="84958-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84958-131">Request</span></span>
<span data-ttu-id="84958-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84958-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="84958-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="84958-133">Response</span></span>
<span data-ttu-id="84958-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84958-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




