---
title: auditEvent aktualisieren
description: Aktualisieren der Eigenschaften eines auditEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 63da381029325977f7cdcf74b8de776c668e0656
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815715"
---
# <a name="update-auditevent"></a><span data-ttu-id="843d9-103">auditEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="843d9-103">Update auditEvent</span></span>

> <span data-ttu-id="843d9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="843d9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="843d9-105">Aktualisieren der Eigenschaften eines [auditEvent](../resources/intune-auditing-auditevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="843d9-105">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="843d9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="843d9-106">Prerequisites</span></span>
<span data-ttu-id="843d9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="843d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="843d9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="843d9-109">Permission type</span></span>|<span data-ttu-id="843d9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="843d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="843d9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="843d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="843d9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="843d9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="843d9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="843d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="843d9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="843d9-114">Not supported.</span></span>|
|<span data-ttu-id="843d9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="843d9-115">Application</span></span>|<span data-ttu-id="843d9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="843d9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="843d9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="843d9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="843d9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="843d9-118">Request headers</span></span>
|<span data-ttu-id="843d9-119">Header</span><span class="sxs-lookup"><span data-stu-id="843d9-119">Header</span></span>|<span data-ttu-id="843d9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="843d9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="843d9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="843d9-121">Authorization</span></span>|<span data-ttu-id="843d9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="843d9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="843d9-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="843d9-123">Accept</span></span>|<span data-ttu-id="843d9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="843d9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="843d9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="843d9-125">Request body</span></span>
<span data-ttu-id="843d9-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [auditEvent](../resources/intune-auditing-auditevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="843d9-126">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="843d9-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="843d9-127">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="843d9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="843d9-128">Property</span></span>|<span data-ttu-id="843d9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="843d9-129">Type</span></span>|<span data-ttu-id="843d9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="843d9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="843d9-131">id</span><span class="sxs-lookup"><span data-stu-id="843d9-131">id</span></span>|<span data-ttu-id="843d9-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="843d9-132">String</span></span>|<span data-ttu-id="843d9-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="843d9-133">Key of the entity.</span></span>|
|<span data-ttu-id="843d9-134">displayName</span><span class="sxs-lookup"><span data-stu-id="843d9-134">displayName</span></span>|<span data-ttu-id="843d9-135">String</span><span class="sxs-lookup"><span data-stu-id="843d9-135">String</span></span>|<span data-ttu-id="843d9-136">Anzeigename des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="843d9-136">Event display name.</span></span>|
|<span data-ttu-id="843d9-137">componentName</span><span class="sxs-lookup"><span data-stu-id="843d9-137">componentName</span></span>|<span data-ttu-id="843d9-138">String</span><span class="sxs-lookup"><span data-stu-id="843d9-138">String</span></span>|<span data-ttu-id="843d9-139">Name der Komponente</span><span class="sxs-lookup"><span data-stu-id="843d9-139">Component name.</span></span>|
|<span data-ttu-id="843d9-140">actor</span><span class="sxs-lookup"><span data-stu-id="843d9-140">actor</span></span>|[<span data-ttu-id="843d9-141">auditActor</span><span class="sxs-lookup"><span data-stu-id="843d9-141">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="843d9-142">AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="843d9-142">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="843d9-143">activity</span><span class="sxs-lookup"><span data-stu-id="843d9-143">activity</span></span>|<span data-ttu-id="843d9-144">String</span><span class="sxs-lookup"><span data-stu-id="843d9-144">String</span></span>|<span data-ttu-id="843d9-145">Anzeigename der Aktivität</span><span class="sxs-lookup"><span data-stu-id="843d9-145">Friendly name of the activity.</span></span>|
|<span data-ttu-id="843d9-146">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="843d9-146">activityDateTime</span></span>|<span data-ttu-id="843d9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="843d9-147">DateTimeOffset</span></span>|<span data-ttu-id="843d9-148">Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format</span><span class="sxs-lookup"><span data-stu-id="843d9-148">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="843d9-149">activityType</span><span class="sxs-lookup"><span data-stu-id="843d9-149">activityType</span></span>|<span data-ttu-id="843d9-150">String</span><span class="sxs-lookup"><span data-stu-id="843d9-150">String</span></span>|<span data-ttu-id="843d9-151">Typ der durchgeführten Aktivität</span><span class="sxs-lookup"><span data-stu-id="843d9-151">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="843d9-152">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="843d9-152">activityOperationType</span></span>|<span data-ttu-id="843d9-153">String</span><span class="sxs-lookup"><span data-stu-id="843d9-153">String</span></span>|<span data-ttu-id="843d9-154">HTTP-Vorgangstyp der Aktivität</span><span class="sxs-lookup"><span data-stu-id="843d9-154">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="843d9-155">activityResult</span><span class="sxs-lookup"><span data-stu-id="843d9-155">activityResult</span></span>|<span data-ttu-id="843d9-156">String</span><span class="sxs-lookup"><span data-stu-id="843d9-156">String</span></span>|<span data-ttu-id="843d9-157">Ergebnis der Aktivität</span><span class="sxs-lookup"><span data-stu-id="843d9-157">The result of the activity.</span></span>|
|<span data-ttu-id="843d9-158">correlationId</span><span class="sxs-lookup"><span data-stu-id="843d9-158">correlationId</span></span>|<span data-ttu-id="843d9-159">Guid</span><span class="sxs-lookup"><span data-stu-id="843d9-159">Guid</span></span>|<span data-ttu-id="843d9-160">ID der Clientanforderung, die zur Korrelation von Aktivitäten im System verwendet wird</span><span class="sxs-lookup"><span data-stu-id="843d9-160">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="843d9-161">resources</span><span class="sxs-lookup"><span data-stu-id="843d9-161">resources</span></span>|<span data-ttu-id="843d9-162">Collection von Objekten des Typs [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="843d9-162">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="843d9-163">Ressourcen, die geändert werden</span><span class="sxs-lookup"><span data-stu-id="843d9-163">Resources being modified.</span></span>|
|<span data-ttu-id="843d9-164">category</span><span class="sxs-lookup"><span data-stu-id="843d9-164">category</span></span>|<span data-ttu-id="843d9-165">String</span><span class="sxs-lookup"><span data-stu-id="843d9-165">String</span></span>|<span data-ttu-id="843d9-166">Überwachungskategorie</span><span class="sxs-lookup"><span data-stu-id="843d9-166">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="843d9-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="843d9-167">Response</span></span>
<span data-ttu-id="843d9-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="843d9-168">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="843d9-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="843d9-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="843d9-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="843d9-170">Request</span></span>
<span data-ttu-id="843d9-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="843d9-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
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

### <a name="response"></a><span data-ttu-id="843d9-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="843d9-172">Response</span></span>
<span data-ttu-id="843d9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="843d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



