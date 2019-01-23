---
title: Aktion „assign“
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9a9d52e62b1d4dd065c1e744593c8e63b695a526
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394362"
---
# <a name="assign-action"></a><span data-ttu-id="3d027-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="3d027-103">assign action</span></span>

> <span data-ttu-id="3d027-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3d027-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d027-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d027-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d027-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3d027-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d027-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3d027-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d027-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d027-108">Prerequisites</span></span>
<span data-ttu-id="3d027-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d027-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d027-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d027-111">Permission type</span></span>|<span data-ttu-id="3d027-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d027-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d027-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d027-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d027-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d027-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d027-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d027-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d027-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d027-116">Not supported.</span></span>|
|<span data-ttu-id="3d027-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d027-117">Application</span></span>|<span data-ttu-id="3d027-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d027-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d027-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d027-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="3d027-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d027-120">Request headers</span></span>
|<span data-ttu-id="3d027-121">Header</span><span class="sxs-lookup"><span data-stu-id="3d027-121">Header</span></span>|<span data-ttu-id="3d027-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3d027-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d027-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3d027-123">Authorization</span></span>|<span data-ttu-id="3d027-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d027-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d027-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3d027-125">Accept</span></span>|<span data-ttu-id="3d027-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d027-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d027-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d027-127">Request body</span></span>
<span data-ttu-id="3d027-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="3d027-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3d027-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3d027-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3d027-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d027-130">Property</span></span>|<span data-ttu-id="3d027-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3d027-131">Type</span></span>|<span data-ttu-id="3d027-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d027-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d027-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="3d027-133">managedEBookAssignments</span></span>|<span data-ttu-id="3d027-134">Collection von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3d027-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="3d027-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3d027-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3d027-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d027-136">Response</span></span>
<span data-ttu-id="3d027-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="3d027-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3d027-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d027-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d027-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d027-139">Request</span></span>
<span data-ttu-id="3d027-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d027-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3d027-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d027-141">Response</span></span>
<span data-ttu-id="3d027-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d027-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




