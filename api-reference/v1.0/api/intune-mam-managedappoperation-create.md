---
title: Erstellen von „managedAppOperation“
description: Diese Methode erstellt ein neues Objekt des Typs managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 297296dae82a172f68b04ca13eeb9200a33aaba0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964207"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="4e9e8-103">Erstellen von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="4e9e8-103">Create managedAppOperation</span></span>

> <span data-ttu-id="4e9e8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4e9e8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e9e8-105">Diese Methode erstellt ein neues Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4e9e8-105">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e9e8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e9e8-106">Prerequisites</span></span>
<span data-ttu-id="4e9e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e9e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e9e8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e9e8-109">Permission type</span></span>|<span data-ttu-id="4e9e8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e9e8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e9e8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e9e8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4e9e8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9e8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e9e8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e9e8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e9e8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e9e8-114">Not supported.</span></span>|
|<span data-ttu-id="4e9e8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e9e8-115">Application</span></span>|<span data-ttu-id="4e9e8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e9e8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e9e8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e9e8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="4e9e8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e9e8-118">Request headers</span></span>
|<span data-ttu-id="4e9e8-119">Header</span><span class="sxs-lookup"><span data-stu-id="4e9e8-119">Header</span></span>|<span data-ttu-id="4e9e8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4e9e8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e9e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e9e8-121">Authorization</span></span>|<span data-ttu-id="4e9e8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4e9e8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e9e8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4e9e8-123">Accept</span></span>|<span data-ttu-id="4e9e8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4e9e8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e9e8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e9e8-125">Request body</span></span>
<span data-ttu-id="4e9e8-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedAppOperation“ an.</span><span class="sxs-lookup"><span data-stu-id="4e9e8-126">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="4e9e8-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedAppOperation“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="4e9e8-127">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="4e9e8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e9e8-128">Property</span></span>|<span data-ttu-id="4e9e8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4e9e8-129">Type</span></span>|<span data-ttu-id="4e9e8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e9e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e9e8-131">displayName</span><span class="sxs-lookup"><span data-stu-id="4e9e8-131">displayName</span></span>|<span data-ttu-id="4e9e8-132">String</span><span class="sxs-lookup"><span data-stu-id="4e9e8-132">String</span></span>|<span data-ttu-id="4e9e8-133">Name des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="4e9e8-133">The operation name.</span></span>|
|<span data-ttu-id="4e9e8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e9e8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="4e9e8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e9e8-135">DateTimeOffset</span></span>|<span data-ttu-id="4e9e8-136">Datum und Uhrzeit der letzten Änderung des App-Vorgangs</span><span class="sxs-lookup"><span data-stu-id="4e9e8-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="4e9e8-137">state</span><span class="sxs-lookup"><span data-stu-id="4e9e8-137">state</span></span>|<span data-ttu-id="4e9e8-138">String</span><span class="sxs-lookup"><span data-stu-id="4e9e8-138">String</span></span>|<span data-ttu-id="4e9e8-139">Aktueller Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="4e9e8-139">The current state of the operation</span></span>|
|<span data-ttu-id="4e9e8-140">id</span><span class="sxs-lookup"><span data-stu-id="4e9e8-140">id</span></span>|<span data-ttu-id="4e9e8-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e9e8-141">String</span></span>|<span data-ttu-id="4e9e8-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4e9e8-142">Key of the entity.</span></span>|
|<span data-ttu-id="4e9e8-143">Version</span><span class="sxs-lookup"><span data-stu-id="4e9e8-143">version</span></span>|<span data-ttu-id="4e9e8-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e9e8-144">String</span></span>|<span data-ttu-id="4e9e8-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="4e9e8-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4e9e8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e9e8-146">Response</span></span>
<span data-ttu-id="4e9e8-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4e9e8-147">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e9e8-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e9e8-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e9e8-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e9e8-149">Request</span></span>
<span data-ttu-id="4e9e8-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e9e8-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="4e9e8-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e9e8-151">Response</span></span>
<span data-ttu-id="4e9e8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e9e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```



