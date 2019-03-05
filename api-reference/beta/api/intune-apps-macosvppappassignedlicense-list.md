---
title: MacOsVppAppAssignedLicenses aufListen
description: AufListen von Eigenschaften und Beziehungen der macOsVppAppAssignedLicense-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7074548158b791dc144dd9dce5a7feb045d123fa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148727"
---
# <a name="list-macosvppappassignedlicenses"></a><span data-ttu-id="badaf-103">MacOsVppAppAssignedLicenses aufListen</span><span class="sxs-lookup"><span data-stu-id="badaf-103">List macOsVppAppAssignedLicenses</span></span>

> <span data-ttu-id="badaf-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="badaf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="badaf-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="badaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="badaf-106">AufListen von Eigenschaften und Beziehungen der [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="badaf-106">List properties and relationships of the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="badaf-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="badaf-107">Prerequisites</span></span>
<span data-ttu-id="badaf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="badaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="badaf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="badaf-110">Permission type</span></span>|<span data-ttu-id="badaf-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="badaf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="badaf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="badaf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="badaf-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="badaf-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="badaf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="badaf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="badaf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="badaf-115">Not supported.</span></span>|
|<span data-ttu-id="badaf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="badaf-116">Application</span></span>|<span data-ttu-id="badaf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="badaf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="badaf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="badaf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="badaf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="badaf-119">Request headers</span></span>
|<span data-ttu-id="badaf-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="badaf-120">Header</span></span>|<span data-ttu-id="badaf-121">Wert</span><span class="sxs-lookup"><span data-stu-id="badaf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="badaf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="badaf-122">Authorization</span></span>|<span data-ttu-id="badaf-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="badaf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="badaf-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="badaf-124">Accept</span></span>|<span data-ttu-id="badaf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="badaf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="badaf-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="badaf-126">Request body</span></span>
<span data-ttu-id="badaf-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="badaf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="badaf-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="badaf-128">Response</span></span>
<span data-ttu-id="badaf-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="badaf-129">If successful, this method returns a `200 OK` response code and a collection of [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="badaf-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="badaf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="badaf-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="badaf-131">Request</span></span>
<span data-ttu-id="badaf-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="badaf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="badaf-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="badaf-133">Response</span></span>
<span data-ttu-id="badaf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="badaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
      "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




