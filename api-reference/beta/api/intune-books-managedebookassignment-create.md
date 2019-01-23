---
title: Erstellen von „managedEBookAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs managedEBookAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1f00c4db40b157359fd04171df6799d56949caa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409559"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="c0063-103">Erstellen von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="c0063-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="c0063-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c0063-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0063-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0063-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0063-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0063-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0063-107">Diese Methode erstellt ein neues Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0063-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0063-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0063-108">Prerequisites</span></span>
<span data-ttu-id="c0063-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0063-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c0063-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0063-111">Permission type</span></span>|<span data-ttu-id="c0063-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0063-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0063-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0063-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0063-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0063-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0063-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0063-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0063-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0063-116">Not supported.</span></span>|
|<span data-ttu-id="c0063-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0063-117">Application</span></span>|<span data-ttu-id="c0063-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0063-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0063-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0063-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c0063-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0063-120">Request headers</span></span>
|<span data-ttu-id="c0063-121">Header</span><span class="sxs-lookup"><span data-stu-id="c0063-121">Header</span></span>|<span data-ttu-id="c0063-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c0063-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0063-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c0063-123">Authorization</span></span>|<span data-ttu-id="c0063-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0063-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0063-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0063-125">Accept</span></span>|<span data-ttu-id="c0063-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0063-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0063-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0063-127">Request body</span></span>
<span data-ttu-id="c0063-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedEBookAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="c0063-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="c0063-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedEBookAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="c0063-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="c0063-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0063-130">Property</span></span>|<span data-ttu-id="c0063-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c0063-131">Type</span></span>|<span data-ttu-id="c0063-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0063-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0063-133">id</span><span class="sxs-lookup"><span data-stu-id="c0063-133">id</span></span>|<span data-ttu-id="c0063-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0063-134">String</span></span>|<span data-ttu-id="c0063-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c0063-135">Key of the entity.</span></span>|
|<span data-ttu-id="c0063-136">target</span><span class="sxs-lookup"><span data-stu-id="c0063-136">target</span></span>|[<span data-ttu-id="c0063-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c0063-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c0063-138">Zuweisungsziel für das E-Book</span><span class="sxs-lookup"><span data-stu-id="c0063-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="c0063-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="c0063-139">installIntent</span></span>|[<span data-ttu-id="c0063-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="c0063-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="c0063-141">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="c0063-141">The install intent for eBook.</span></span> <span data-ttu-id="c0063-142">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="c0063-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="c0063-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0063-143">Response</span></span>
<span data-ttu-id="c0063-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c0063-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0063-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0063-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0063-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0063-146">Request</span></span>
<span data-ttu-id="c0063-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0063-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="c0063-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0063-148">Response</span></span>
<span data-ttu-id="c0063-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0063-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```




