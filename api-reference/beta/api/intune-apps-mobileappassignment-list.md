---
title: Auflisten von „mobileAppAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs mobileAppAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41c9b883b50b30a4cda6033efb45e73eb251f4cf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141139"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="ffb31-103">Auflisten von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="ffb31-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="ffb31-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ffb31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffb31-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ffb31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffb31-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ffb31-106">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffb31-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ffb31-107">Prerequisites</span></span>
<span data-ttu-id="ffb31-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffb31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ffb31-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ffb31-110">Permission type</span></span>|<span data-ttu-id="ffb31-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ffb31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffb31-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ffb31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffb31-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffb31-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ffb31-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ffb31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffb31-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffb31-115">Not supported.</span></span>|
|<span data-ttu-id="ffb31-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffb31-116">Application</span></span>|<span data-ttu-id="ffb31-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffb31-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffb31-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffb31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ffb31-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ffb31-119">Request headers</span></span>
|<span data-ttu-id="ffb31-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ffb31-120">Header</span></span>|<span data-ttu-id="ffb31-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ffb31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffb31-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffb31-122">Authorization</span></span>|<span data-ttu-id="ffb31-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ffb31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffb31-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ffb31-124">Accept</span></span>|<span data-ttu-id="ffb31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffb31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb31-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ffb31-126">Request body</span></span>
<span data-ttu-id="ffb31-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ffb31-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffb31-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffb31-128">Response</span></span>
<span data-ttu-id="ffb31-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ffb31-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb31-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ffb31-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffb31-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffb31-131">Request</span></span>
<span data-ttu-id="ffb31-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ffb31-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="ffb31-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffb31-133">Response</span></span>
<span data-ttu-id="ffb31-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffb31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```




