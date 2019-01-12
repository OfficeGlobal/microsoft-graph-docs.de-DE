---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 01af5e970a56f871078a26adc3514a07f97b5d57
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958488"
---
# <a name="assign-action"></a><span data-ttu-id="5baa7-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="5baa7-103">assign action</span></span>

> <span data-ttu-id="5baa7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5baa7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5baa7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5baa7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5baa7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5baa7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5baa7-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5baa7-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5baa7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5baa7-108">Prerequisites</span></span>
<span data-ttu-id="5baa7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5baa7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5baa7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5baa7-111">Permission type</span></span>|<span data-ttu-id="5baa7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5baa7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5baa7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5baa7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5baa7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5baa7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5baa7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5baa7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5baa7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5baa7-116">Not supported.</span></span>|
|<span data-ttu-id="5baa7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5baa7-117">Application</span></span>|<span data-ttu-id="5baa7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5baa7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5baa7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5baa7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5baa7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5baa7-120">Request headers</span></span>
|<span data-ttu-id="5baa7-121">Header</span><span class="sxs-lookup"><span data-stu-id="5baa7-121">Header</span></span>|<span data-ttu-id="5baa7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5baa7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5baa7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5baa7-123">Authorization</span></span>|<span data-ttu-id="5baa7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5baa7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5baa7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5baa7-125">Accept</span></span>|<span data-ttu-id="5baa7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5baa7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5baa7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5baa7-127">Request body</span></span>
<span data-ttu-id="5baa7-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="5baa7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5baa7-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5baa7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5baa7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5baa7-130">Property</span></span>|<span data-ttu-id="5baa7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5baa7-131">Type</span></span>|<span data-ttu-id="5baa7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5baa7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5baa7-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="5baa7-133">managedEBookAssignments</span></span>|<span data-ttu-id="5baa7-134">Collection von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5baa7-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5baa7-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5baa7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5baa7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5baa7-136">Response</span></span>
<span data-ttu-id="5baa7-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="5baa7-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5baa7-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5baa7-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="5baa7-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5baa7-139">Request</span></span>
<span data-ttu-id="5baa7-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5baa7-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5baa7-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="5baa7-141">Response</span></span>
<span data-ttu-id="5baa7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5baa7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





