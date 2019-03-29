---
title: Aktion zuweisen
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94c50cf4e3f880f61f1e392d9166c6dfe7a6f5ac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978626"
---
# <a name="assign-action"></a><span data-ttu-id="0a21d-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="0a21d-103">assign action</span></span>

> <span data-ttu-id="0a21d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0a21d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a21d-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0a21d-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a21d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0a21d-106">Prerequisites</span></span>
<span data-ttu-id="0a21d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a21d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a21d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a21d-109">Permission type</span></span>|<span data-ttu-id="0a21d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a21d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a21d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a21d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a21d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a21d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a21d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a21d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a21d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a21d-114">Not supported.</span></span>|
|<span data-ttu-id="0a21d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a21d-115">Application</span></span>|<span data-ttu-id="0a21d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a21d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a21d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a21d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0a21d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a21d-118">Request headers</span></span>
|<span data-ttu-id="0a21d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0a21d-119">Header</span></span>|<span data-ttu-id="0a21d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0a21d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a21d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a21d-121">Authorization</span></span>|<span data-ttu-id="0a21d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a21d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a21d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0a21d-123">Accept</span></span>|<span data-ttu-id="0a21d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a21d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a21d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a21d-125">Request body</span></span>
<span data-ttu-id="0a21d-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="0a21d-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0a21d-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="0a21d-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0a21d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a21d-128">Property</span></span>|<span data-ttu-id="0a21d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0a21d-129">Type</span></span>|<span data-ttu-id="0a21d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a21d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a21d-131">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="0a21d-131">managedEBookAssignments</span></span>|<span data-ttu-id="0a21d-132">Collection von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0a21d-132">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="0a21d-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0a21d-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0a21d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a21d-134">Response</span></span>
<span data-ttu-id="0a21d-135">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a21d-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a21d-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a21d-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a21d-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a21d-137">Request</span></span>
<span data-ttu-id="0a21d-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a21d-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assign

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

### <a name="response"></a><span data-ttu-id="0a21d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a21d-139">Response</span></span>
<span data-ttu-id="0a21d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a21d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



