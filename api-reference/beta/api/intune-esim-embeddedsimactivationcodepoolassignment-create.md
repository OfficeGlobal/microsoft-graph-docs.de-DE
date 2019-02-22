---
title: EmbeddedSIMActivationCodePoolAssignment erstellen
description: Erstellen eines neuen embeddedSIMActivationCodePoolAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02b4c39b4ca999780a620510c38fc80036e02ee1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169622"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="ccab6-103">EmbeddedSIMActivationCodePoolAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="ccab6-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="ccab6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ccab6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccab6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ccab6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccab6-106">Erstellen eines neuen [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ccab6-106">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccab6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ccab6-107">Prerequisites</span></span>
<span data-ttu-id="ccab6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ccab6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ccab6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ccab6-110">Permission type</span></span>|<span data-ttu-id="ccab6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ccab6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccab6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ccab6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccab6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccab6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccab6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ccab6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccab6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ccab6-115">Not supported.</span></span>|
|<span data-ttu-id="ccab6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ccab6-116">Application</span></span>|<span data-ttu-id="ccab6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ccab6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccab6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccab6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ccab6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ccab6-119">Request headers</span></span>
|<span data-ttu-id="ccab6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ccab6-120">Header</span></span>|<span data-ttu-id="ccab6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ccab6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccab6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccab6-122">Authorization</span></span>|<span data-ttu-id="ccab6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ccab6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccab6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ccab6-124">Accept</span></span>|<span data-ttu-id="ccab6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ccab6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccab6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ccab6-126">Request body</span></span>
<span data-ttu-id="ccab6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das embeddedSIMActivationCodePoolAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ccab6-127">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="ccab6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der embeddedSIMActivationCodePoolAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ccab6-128">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="ccab6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ccab6-129">Property</span></span>|<span data-ttu-id="ccab6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ccab6-130">Type</span></span>|<span data-ttu-id="ccab6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ccab6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccab6-132">id</span><span class="sxs-lookup"><span data-stu-id="ccab6-132">id</span></span>|<span data-ttu-id="ccab6-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ccab6-133">String</span></span>|<span data-ttu-id="ccab6-134">Eindeutige ID für den eingebetteten SIM-Aktivierungscode-Pool-Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="ccab6-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="ccab6-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="ccab6-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="ccab6-136">target</span><span class="sxs-lookup"><span data-stu-id="ccab6-136">target</span></span>|[<span data-ttu-id="ccab6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ccab6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ccab6-138">Der Typ der Gruppen, die vom eingebetteten SIM-Aktivierungscode Pool abzielen.</span><span class="sxs-lookup"><span data-stu-id="ccab6-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="ccab6-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccab6-139">Response</span></span>
<span data-ttu-id="ccab6-140">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ccab6-140">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccab6-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ccab6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccab6-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccab6-142">Request</span></span>
<span data-ttu-id="ccab6-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ccab6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ccab6-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccab6-144">Response</span></span>
<span data-ttu-id="ccab6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ccab6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




