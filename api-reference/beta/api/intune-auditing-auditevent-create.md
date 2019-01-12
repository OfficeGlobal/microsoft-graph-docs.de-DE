---
title: Erstellen von „auditEvent“
description: Diese Methode erstellt ein neues Objekt des Typs auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b6b673e2c7090ecfee3368d76f4690dd309ffdd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980279"
---
# <a name="create-auditevent"></a><span data-ttu-id="199f6-103">Erstellen von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="199f6-103">Create auditEvent</span></span>

> <span data-ttu-id="199f6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="199f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="199f6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="199f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="199f6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="199f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="199f6-107">Diese Methode erstellt ein neues Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="199f6-107">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="199f6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="199f6-108">Prerequisites</span></span>
<span data-ttu-id="199f6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="199f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="199f6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="199f6-111">Permission type</span></span>|<span data-ttu-id="199f6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="199f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="199f6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="199f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="199f6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="199f6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="199f6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="199f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="199f6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="199f6-116">Not supported.</span></span>|
|<span data-ttu-id="199f6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="199f6-117">Application</span></span>|<span data-ttu-id="199f6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="199f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="199f6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="199f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="199f6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="199f6-120">Request headers</span></span>
|<span data-ttu-id="199f6-121">Header</span><span class="sxs-lookup"><span data-stu-id="199f6-121">Header</span></span>|<span data-ttu-id="199f6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="199f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="199f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="199f6-123">Authorization</span></span>|<span data-ttu-id="199f6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="199f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="199f6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="199f6-125">Accept</span></span>|<span data-ttu-id="199f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="199f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="199f6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="199f6-127">Request body</span></span>
<span data-ttu-id="199f6-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „auditEvent“ an.</span><span class="sxs-lookup"><span data-stu-id="199f6-128">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="199f6-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „auditEvent“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="199f6-129">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="199f6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="199f6-130">Property</span></span>|<span data-ttu-id="199f6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="199f6-131">Type</span></span>|<span data-ttu-id="199f6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="199f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="199f6-133">id</span><span class="sxs-lookup"><span data-stu-id="199f6-133">id</span></span>|<span data-ttu-id="199f6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="199f6-134">String</span></span>|<span data-ttu-id="199f6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="199f6-135">Key of the entity.</span></span>|
|<span data-ttu-id="199f6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="199f6-136">displayName</span></span>|<span data-ttu-id="199f6-137">String</span><span class="sxs-lookup"><span data-stu-id="199f6-137">String</span></span>|<span data-ttu-id="199f6-138">Anzeigename des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="199f6-138">Event display name.</span></span>|
|<span data-ttu-id="199f6-139">componentName</span><span class="sxs-lookup"><span data-stu-id="199f6-139">componentName</span></span>|<span data-ttu-id="199f6-140">String</span><span class="sxs-lookup"><span data-stu-id="199f6-140">String</span></span>|<span data-ttu-id="199f6-141">Name der Komponente</span><span class="sxs-lookup"><span data-stu-id="199f6-141">Component name.</span></span>|
|<span data-ttu-id="199f6-142">actor</span><span class="sxs-lookup"><span data-stu-id="199f6-142">actor</span></span>|[<span data-ttu-id="199f6-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="199f6-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="199f6-144">AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="199f6-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="199f6-145">activity</span><span class="sxs-lookup"><span data-stu-id="199f6-145">activity</span></span>|<span data-ttu-id="199f6-146">String</span><span class="sxs-lookup"><span data-stu-id="199f6-146">String</span></span>|<span data-ttu-id="199f6-147">Anzeigename der Aktivität</span><span class="sxs-lookup"><span data-stu-id="199f6-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="199f6-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="199f6-148">activityDateTime</span></span>|<span data-ttu-id="199f6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="199f6-149">DateTimeOffset</span></span>|<span data-ttu-id="199f6-150">Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format</span><span class="sxs-lookup"><span data-stu-id="199f6-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="199f6-151">activityType</span><span class="sxs-lookup"><span data-stu-id="199f6-151">activityType</span></span>|<span data-ttu-id="199f6-152">String</span><span class="sxs-lookup"><span data-stu-id="199f6-152">String</span></span>|<span data-ttu-id="199f6-153">Typ der durchgeführten Aktivität</span><span class="sxs-lookup"><span data-stu-id="199f6-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="199f6-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="199f6-154">activityOperationType</span></span>|<span data-ttu-id="199f6-155">String</span><span class="sxs-lookup"><span data-stu-id="199f6-155">String</span></span>|<span data-ttu-id="199f6-156">HTTP-Vorgangstyp der Aktivität</span><span class="sxs-lookup"><span data-stu-id="199f6-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="199f6-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="199f6-157">activityResult</span></span>|<span data-ttu-id="199f6-158">String</span><span class="sxs-lookup"><span data-stu-id="199f6-158">String</span></span>|<span data-ttu-id="199f6-159">Ergebnis der Aktivität</span><span class="sxs-lookup"><span data-stu-id="199f6-159">The result of the activity.</span></span>|
|<span data-ttu-id="199f6-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="199f6-160">correlationId</span></span>|<span data-ttu-id="199f6-161">Guid</span><span class="sxs-lookup"><span data-stu-id="199f6-161">Guid</span></span>|<span data-ttu-id="199f6-162">ID der Clientanforderung, die zur Korrelation von Aktivitäten im System verwendet wird</span><span class="sxs-lookup"><span data-stu-id="199f6-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="199f6-163">resources</span><span class="sxs-lookup"><span data-stu-id="199f6-163">resources</span></span>|<span data-ttu-id="199f6-164">Collection von Objekten des Typs [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="199f6-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="199f6-165">Ressourcen, die geändert werden</span><span class="sxs-lookup"><span data-stu-id="199f6-165">Resources being modified.</span></span>|
|<span data-ttu-id="199f6-166">category</span><span class="sxs-lookup"><span data-stu-id="199f6-166">category</span></span>|<span data-ttu-id="199f6-167">String</span><span class="sxs-lookup"><span data-stu-id="199f6-167">String</span></span>|<span data-ttu-id="199f6-168">Überwachungskategorie</span><span class="sxs-lookup"><span data-stu-id="199f6-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="199f6-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="199f6-169">Response</span></span>
<span data-ttu-id="199f6-170">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="199f6-170">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="199f6-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="199f6-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="199f6-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="199f6-172">Request</span></span>
<span data-ttu-id="199f6-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="199f6-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
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

### <a name="response"></a><span data-ttu-id="199f6-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="199f6-174">Response</span></span>
<span data-ttu-id="199f6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="199f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





