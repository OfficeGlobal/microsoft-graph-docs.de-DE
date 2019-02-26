---
title: mobileAppAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des mobileAppAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e214d8c3076121b7c4e053488755afd0ad9154cd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261481"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="0e4e1-103">mobileAppAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="0e4e1-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="0e4e1-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0e4e1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e4e1-105">Lesen von Eigenschaften und Beziehungen des [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e4e1-105">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e4e1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0e4e1-106">Prerequisites</span></span>
<span data-ttu-id="0e4e1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e4e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0e4e1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e4e1-109">Permission type</span></span>|<span data-ttu-id="0e4e1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e4e1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e4e1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e4e1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e4e1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e4e1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0e4e1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e4e1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e4e1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e4e1-114">Not supported.</span></span>|
|<span data-ttu-id="0e4e1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e4e1-115">Application</span></span>|<span data-ttu-id="0e4e1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e4e1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e4e1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e4e1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e4e1-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0e4e1-118">Optional query parameters</span></span>
<span data-ttu-id="0e4e1-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e4e1-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e4e1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e4e1-120">Request headers</span></span>
|<span data-ttu-id="0e4e1-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0e4e1-121">Header</span></span>|<span data-ttu-id="0e4e1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0e4e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e4e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e4e1-123">Authorization</span></span>|<span data-ttu-id="0e4e1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0e4e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e4e1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0e4e1-125">Accept</span></span>|<span data-ttu-id="0e4e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e4e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e4e1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e4e1-127">Request body</span></span>
<span data-ttu-id="0e4e1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0e4e1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e4e1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e4e1-129">Response</span></span>
<span data-ttu-id="0e4e1-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e4e1-130">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e4e1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e4e1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e4e1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e4e1-132">Request</span></span>
<span data-ttu-id="0e4e1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e4e1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="0e4e1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e4e1-134">Response</span></span>
<span data-ttu-id="0e4e1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e4e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": {
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
}
```



