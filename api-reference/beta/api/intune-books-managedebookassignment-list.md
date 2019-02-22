---
title: Auflisten von „managedEBookAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedEBookAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c71c4804f2f75a1a2ea5d283f2256b72575ccacc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168789"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="c11dd-103">Auflisten von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="c11dd-103">List managedEBookAssignments</span></span>

> <span data-ttu-id="c11dd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c11dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c11dd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c11dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c11dd-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="c11dd-106">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c11dd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c11dd-107">Prerequisites</span></span>
<span data-ttu-id="c11dd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c11dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c11dd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c11dd-110">Permission type</span></span>|<span data-ttu-id="c11dd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c11dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c11dd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c11dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c11dd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c11dd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c11dd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c11dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c11dd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c11dd-115">Not supported.</span></span>|
|<span data-ttu-id="c11dd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c11dd-116">Application</span></span>|<span data-ttu-id="c11dd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c11dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c11dd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c11dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c11dd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c11dd-119">Request headers</span></span>
|<span data-ttu-id="c11dd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c11dd-120">Header</span></span>|<span data-ttu-id="c11dd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c11dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c11dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c11dd-122">Authorization</span></span>|<span data-ttu-id="c11dd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c11dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c11dd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c11dd-124">Accept</span></span>|<span data-ttu-id="c11dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c11dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c11dd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c11dd-126">Request body</span></span>
<span data-ttu-id="c11dd-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c11dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c11dd-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c11dd-128">Response</span></span>
<span data-ttu-id="c11dd-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c11dd-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c11dd-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c11dd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c11dd-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c11dd-131">Request</span></span>
<span data-ttu-id="c11dd-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c11dd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="c11dd-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c11dd-133">Response</span></span>
<span data-ttu-id="c11dd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c11dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 300

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```




