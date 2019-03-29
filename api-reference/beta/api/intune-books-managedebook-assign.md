---
title: Aktion zuweisen
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fdb01aa0c85864081b27b6ab00e56ae6af55302
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980985"
---
# <a name="assign-action"></a><span data-ttu-id="e8f1d-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="e8f1d-103">assign action</span></span>

> <span data-ttu-id="e8f1d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8f1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8f1d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e8f1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8f1d-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e8f1d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8f1d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e8f1d-107">Prerequisites</span></span>
<span data-ttu-id="e8f1d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8f1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8f1d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8f1d-110">Permission type</span></span>|<span data-ttu-id="e8f1d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8f1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8f1d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8f1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8f1d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8f1d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e8f1d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8f1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8f1d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8f1d-115">Not supported.</span></span>|
|<span data-ttu-id="e8f1d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8f1d-116">Application</span></span>|<span data-ttu-id="e8f1d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8f1d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8f1d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8f1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e8f1d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8f1d-119">Request headers</span></span>
|<span data-ttu-id="e8f1d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e8f1d-120">Header</span></span>|<span data-ttu-id="e8f1d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e8f1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8f1d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8f1d-122">Authorization</span></span>|<span data-ttu-id="e8f1d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e8f1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8f1d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e8f1d-124">Accept</span></span>|<span data-ttu-id="e8f1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8f1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8f1d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8f1d-126">Request body</span></span>
<span data-ttu-id="e8f1d-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="e8f1d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e8f1d-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e8f1d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e8f1d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e8f1d-129">Property</span></span>|<span data-ttu-id="e8f1d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e8f1d-130">Type</span></span>|<span data-ttu-id="e8f1d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8f1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8f1d-132">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="e8f1d-132">managedEBookAssignments</span></span>|<span data-ttu-id="e8f1d-133">Collection von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e8f1d-133">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="e8f1d-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e8f1d-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e8f1d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8f1d-135">Response</span></span>
<span data-ttu-id="e8f1d-136">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8f1d-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8f1d-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8f1d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8f1d-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8f1d-138">Request</span></span>
<span data-ttu-id="e8f1d-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8f1d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 318

{
  "managedEBookAssignments": [
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

### <a name="response"></a><span data-ttu-id="e8f1d-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8f1d-140">Response</span></span>
<span data-ttu-id="e8f1d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8f1d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




