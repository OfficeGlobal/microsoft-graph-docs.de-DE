---
title: Auflisten von „managedEBookAssignment“
description: Auflisten von Eigenschaften und Beziehungen der managedEBookAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed2fdff885f57dd38690844a2f9a09e26177e775
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980957"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="1c5c6-103">Auflisten von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="1c5c6-103">List managedEBookAssignments</span></span>

> <span data-ttu-id="1c5c6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c5c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c5c6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1c5c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c5c6-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="1c5c6-106">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c5c6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c5c6-107">Prerequisites</span></span>
<span data-ttu-id="1c5c6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c5c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c5c6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c5c6-110">Permission type</span></span>|<span data-ttu-id="1c5c6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c5c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c5c6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c5c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c5c6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c5c6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1c5c6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c5c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c5c6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c5c6-115">Not supported.</span></span>|
|<span data-ttu-id="1c5c6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c5c6-116">Application</span></span>|<span data-ttu-id="1c5c6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c5c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c5c6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c5c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1c5c6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c5c6-119">Request headers</span></span>
|<span data-ttu-id="1c5c6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c5c6-120">Header</span></span>|<span data-ttu-id="1c5c6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1c5c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c5c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c5c6-122">Authorization</span></span>|<span data-ttu-id="1c5c6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c5c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c5c6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1c5c6-124">Accept</span></span>|<span data-ttu-id="1c5c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c5c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c5c6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c5c6-126">Request body</span></span>
<span data-ttu-id="1c5c6-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c5c6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c5c6-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c5c6-128">Response</span></span>
<span data-ttu-id="1c5c6-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1c5c6-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c5c6-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c5c6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c5c6-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c5c6-131">Request</span></span>
<span data-ttu-id="1c5c6-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c5c6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="1c5c6-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c5c6-133">Response</span></span>
<span data-ttu-id="1c5c6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c5c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




