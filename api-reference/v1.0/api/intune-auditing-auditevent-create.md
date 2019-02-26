---
title: Erstellen von „auditEvent“
description: Diese Methode erstellt ein neues Objekt des Typs auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f85c7d8e9ff94ad5f6ae3a10df695c4cbb1f5d6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255972"
---
# <a name="create-auditevent"></a><span data-ttu-id="983d6-103">Erstellen von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="983d6-103">Create auditEvent</span></span>

> <span data-ttu-id="983d6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="983d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="983d6-105">Diese Methode erstellt ein neues Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="983d6-105">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="983d6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="983d6-106">Prerequisites</span></span>
<span data-ttu-id="983d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="983d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="983d6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="983d6-109">Permission type</span></span>|<span data-ttu-id="983d6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="983d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="983d6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="983d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="983d6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="983d6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="983d6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="983d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="983d6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="983d6-114">Not supported.</span></span>|
|<span data-ttu-id="983d6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="983d6-115">Application</span></span>|<span data-ttu-id="983d6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="983d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="983d6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="983d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="983d6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="983d6-118">Request headers</span></span>
|<span data-ttu-id="983d6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="983d6-119">Header</span></span>|<span data-ttu-id="983d6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="983d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="983d6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="983d6-121">Authorization</span></span>|<span data-ttu-id="983d6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="983d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="983d6-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="983d6-123">Accept</span></span>|<span data-ttu-id="983d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="983d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="983d6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="983d6-125">Request body</span></span>
<span data-ttu-id="983d6-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „auditEvent“ an.</span><span class="sxs-lookup"><span data-stu-id="983d6-126">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="983d6-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „auditEvent“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="983d6-127">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="983d6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="983d6-128">Property</span></span>|<span data-ttu-id="983d6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="983d6-129">Type</span></span>|<span data-ttu-id="983d6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="983d6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="983d6-131">id</span><span class="sxs-lookup"><span data-stu-id="983d6-131">id</span></span>|<span data-ttu-id="983d6-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="983d6-132">String</span></span>|<span data-ttu-id="983d6-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="983d6-133">Key of the entity.</span></span>|
|<span data-ttu-id="983d6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="983d6-134">displayName</span></span>|<span data-ttu-id="983d6-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="983d6-135">String</span></span>|<span data-ttu-id="983d6-136">Anzeigename des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="983d6-136">Event display name.</span></span>|
|<span data-ttu-id="983d6-137">componentName</span><span class="sxs-lookup"><span data-stu-id="983d6-137">componentName</span></span>|<span data-ttu-id="983d6-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="983d6-138">String</span></span>|<span data-ttu-id="983d6-139">Name der Komponente</span><span class="sxs-lookup"><span data-stu-id="983d6-139">Component name.</span></span>|
|<span data-ttu-id="983d6-140">actor</span><span class="sxs-lookup"><span data-stu-id="983d6-140">actor</span></span>|[<span data-ttu-id="983d6-141">auditActor</span><span class="sxs-lookup"><span data-stu-id="983d6-141">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="983d6-142">AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="983d6-142">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="983d6-143">activity</span><span class="sxs-lookup"><span data-stu-id="983d6-143">activity</span></span>|<span data-ttu-id="983d6-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="983d6-144">String</span></span>|<span data-ttu-id="983d6-145">Anzeigename der Aktivität</span><span class="sxs-lookup"><span data-stu-id="983d6-145">Friendly name of the activity.</span></span>|
|<span data-ttu-id="983d6-146">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="983d6-146">activityDateTime</span></span>|<span data-ttu-id="983d6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="983d6-147">DateTimeOffset</span></span>|<span data-ttu-id="983d6-148">Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format</span><span class="sxs-lookup"><span data-stu-id="983d6-148">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="983d6-149">activityType</span><span class="sxs-lookup"><span data-stu-id="983d6-149">activityType</span></span>|<span data-ttu-id="983d6-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="983d6-150">String</span></span>|<span data-ttu-id="983d6-151">Typ der durchgeführten Aktivität</span><span class="sxs-lookup"><span data-stu-id="983d6-151">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="983d6-152">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="983d6-152">activityOperationType</span></span>|<span data-ttu-id="983d6-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="983d6-153">String</span></span>|<span data-ttu-id="983d6-154">HTTP-Vorgangstyp der Aktivität</span><span class="sxs-lookup"><span data-stu-id="983d6-154">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="983d6-155">activityResult</span><span class="sxs-lookup"><span data-stu-id="983d6-155">activityResult</span></span>|<span data-ttu-id="983d6-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="983d6-156">String</span></span>|<span data-ttu-id="983d6-157">Ergebnis der Aktivität</span><span class="sxs-lookup"><span data-stu-id="983d6-157">The result of the activity.</span></span>|
|<span data-ttu-id="983d6-158">correlationId</span><span class="sxs-lookup"><span data-stu-id="983d6-158">correlationId</span></span>|<span data-ttu-id="983d6-159">Guid</span><span class="sxs-lookup"><span data-stu-id="983d6-159">Guid</span></span>|<span data-ttu-id="983d6-160">ID der Clientanforderung, die zur Korrelation von Aktivitäten im System verwendet wird</span><span class="sxs-lookup"><span data-stu-id="983d6-160">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="983d6-161">resources</span><span class="sxs-lookup"><span data-stu-id="983d6-161">resources</span></span>|<span data-ttu-id="983d6-162">Collection von Objekten des Typs [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="983d6-162">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="983d6-163">Ressourcen, die geändert werden</span><span class="sxs-lookup"><span data-stu-id="983d6-163">Resources being modified.</span></span>|
|<span data-ttu-id="983d6-164">category</span><span class="sxs-lookup"><span data-stu-id="983d6-164">category</span></span>|<span data-ttu-id="983d6-165">String</span><span class="sxs-lookup"><span data-stu-id="983d6-165">String</span></span>|<span data-ttu-id="983d6-166">Überwachungskategorie</span><span class="sxs-lookup"><span data-stu-id="983d6-166">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="983d6-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="983d6-167">Response</span></span>
<span data-ttu-id="983d6-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="983d6-168">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="983d6-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="983d6-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="983d6-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="983d6-170">Request</span></span>
<span data-ttu-id="983d6-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="983d6-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1390

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="983d6-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="983d6-172">Response</span></span>
<span data-ttu-id="983d6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="983d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```



