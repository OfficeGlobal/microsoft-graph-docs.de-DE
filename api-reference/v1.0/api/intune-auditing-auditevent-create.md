---
title: Erstellen von „auditEvent“
description: Diese Methode erstellt ein neues Objekt des Typs auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 696368ca8c129f1e2fd51682e037626bb89469aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991167"
---
# <a name="create-auditevent"></a><span data-ttu-id="eb84e-103">Erstellen von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="eb84e-103">Create auditEvent</span></span>

> <span data-ttu-id="eb84e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb84e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb84e-105">Diese Methode erstellt ein neues Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="eb84e-105">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb84e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb84e-106">Prerequisites</span></span>
<span data-ttu-id="eb84e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb84e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb84e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb84e-109">Permission type</span></span>|<span data-ttu-id="eb84e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb84e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb84e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb84e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb84e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb84e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eb84e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb84e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb84e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb84e-114">Not supported.</span></span>|
|<span data-ttu-id="eb84e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb84e-115">Application</span></span>|<span data-ttu-id="eb84e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb84e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb84e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb84e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="eb84e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb84e-118">Request headers</span></span>
|<span data-ttu-id="eb84e-119">Header</span><span class="sxs-lookup"><span data-stu-id="eb84e-119">Header</span></span>|<span data-ttu-id="eb84e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="eb84e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb84e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb84e-121">Authorization</span></span>|<span data-ttu-id="eb84e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb84e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb84e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eb84e-123">Accept</span></span>|<span data-ttu-id="eb84e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eb84e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb84e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb84e-125">Request body</span></span>
<span data-ttu-id="eb84e-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „auditEvent“ an.</span><span class="sxs-lookup"><span data-stu-id="eb84e-126">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="eb84e-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „auditEvent“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="eb84e-127">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="eb84e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb84e-128">Property</span></span>|<span data-ttu-id="eb84e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="eb84e-129">Type</span></span>|<span data-ttu-id="eb84e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb84e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb84e-131">id</span><span class="sxs-lookup"><span data-stu-id="eb84e-131">id</span></span>|<span data-ttu-id="eb84e-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb84e-132">String</span></span>|<span data-ttu-id="eb84e-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eb84e-133">Key of the entity.</span></span>|
|<span data-ttu-id="eb84e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="eb84e-134">displayName</span></span>|<span data-ttu-id="eb84e-135">String</span><span class="sxs-lookup"><span data-stu-id="eb84e-135">String</span></span>|<span data-ttu-id="eb84e-136">Anzeigename des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="eb84e-136">Event display name.</span></span>|
|<span data-ttu-id="eb84e-137">componentName</span><span class="sxs-lookup"><span data-stu-id="eb84e-137">componentName</span></span>|<span data-ttu-id="eb84e-138">String</span><span class="sxs-lookup"><span data-stu-id="eb84e-138">String</span></span>|<span data-ttu-id="eb84e-139">Name der Komponente</span><span class="sxs-lookup"><span data-stu-id="eb84e-139">Component name.</span></span>|
|<span data-ttu-id="eb84e-140">actor</span><span class="sxs-lookup"><span data-stu-id="eb84e-140">actor</span></span>|[<span data-ttu-id="eb84e-141">auditActor</span><span class="sxs-lookup"><span data-stu-id="eb84e-141">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="eb84e-142">AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="eb84e-142">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="eb84e-143">activity</span><span class="sxs-lookup"><span data-stu-id="eb84e-143">activity</span></span>|<span data-ttu-id="eb84e-144">String</span><span class="sxs-lookup"><span data-stu-id="eb84e-144">String</span></span>|<span data-ttu-id="eb84e-145">Anzeigename der Aktivität</span><span class="sxs-lookup"><span data-stu-id="eb84e-145">Friendly name of the activity.</span></span>|
|<span data-ttu-id="eb84e-146">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="eb84e-146">activityDateTime</span></span>|<span data-ttu-id="eb84e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb84e-147">DateTimeOffset</span></span>|<span data-ttu-id="eb84e-148">Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format</span><span class="sxs-lookup"><span data-stu-id="eb84e-148">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="eb84e-149">activityType</span><span class="sxs-lookup"><span data-stu-id="eb84e-149">activityType</span></span>|<span data-ttu-id="eb84e-150">String</span><span class="sxs-lookup"><span data-stu-id="eb84e-150">String</span></span>|<span data-ttu-id="eb84e-151">Typ der durchgeführten Aktivität</span><span class="sxs-lookup"><span data-stu-id="eb84e-151">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="eb84e-152">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="eb84e-152">activityOperationType</span></span>|<span data-ttu-id="eb84e-153">String</span><span class="sxs-lookup"><span data-stu-id="eb84e-153">String</span></span>|<span data-ttu-id="eb84e-154">HTTP-Vorgangstyp der Aktivität</span><span class="sxs-lookup"><span data-stu-id="eb84e-154">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="eb84e-155">activityResult</span><span class="sxs-lookup"><span data-stu-id="eb84e-155">activityResult</span></span>|<span data-ttu-id="eb84e-156">String</span><span class="sxs-lookup"><span data-stu-id="eb84e-156">String</span></span>|<span data-ttu-id="eb84e-157">Ergebnis der Aktivität</span><span class="sxs-lookup"><span data-stu-id="eb84e-157">The result of the activity.</span></span>|
|<span data-ttu-id="eb84e-158">correlationId</span><span class="sxs-lookup"><span data-stu-id="eb84e-158">correlationId</span></span>|<span data-ttu-id="eb84e-159">Guid</span><span class="sxs-lookup"><span data-stu-id="eb84e-159">Guid</span></span>|<span data-ttu-id="eb84e-160">ID der Clientanforderung, die zur Korrelation von Aktivitäten im System verwendet wird</span><span class="sxs-lookup"><span data-stu-id="eb84e-160">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="eb84e-161">resources</span><span class="sxs-lookup"><span data-stu-id="eb84e-161">resources</span></span>|<span data-ttu-id="eb84e-162">Collection von Objekten des Typs [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="eb84e-162">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="eb84e-163">Ressourcen, die geändert werden</span><span class="sxs-lookup"><span data-stu-id="eb84e-163">Resources being modified.</span></span>|
|<span data-ttu-id="eb84e-164">category</span><span class="sxs-lookup"><span data-stu-id="eb84e-164">category</span></span>|<span data-ttu-id="eb84e-165">String</span><span class="sxs-lookup"><span data-stu-id="eb84e-165">String</span></span>|<span data-ttu-id="eb84e-166">Überwachungskategorie</span><span class="sxs-lookup"><span data-stu-id="eb84e-166">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="eb84e-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb84e-167">Response</span></span>
<span data-ttu-id="eb84e-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eb84e-168">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb84e-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb84e-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb84e-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb84e-170">Request</span></span>
<span data-ttu-id="eb84e-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb84e-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb84e-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb84e-172">Response</span></span>
<span data-ttu-id="eb84e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb84e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



