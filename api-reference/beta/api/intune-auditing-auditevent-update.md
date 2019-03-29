---
title: auditEvent aktualisieren
description: Aktualisieren der Eigenschaften eines auditEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdc8a9e13f231b1cf424ada6fbcdfaaacd722cc1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981202"
---
# <a name="update-auditevent"></a><span data-ttu-id="a9bb3-103">auditEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a9bb3-103">Update auditEvent</span></span>

> <span data-ttu-id="a9bb3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9bb3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9bb3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a9bb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9bb3-106">Aktualisieren der Eigenschaften eines [auditEvent](../resources/intune-auditing-auditevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a9bb3-106">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9bb3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a9bb3-107">Prerequisites</span></span>
<span data-ttu-id="a9bb3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9bb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9bb3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9bb3-110">Permission type</span></span>|<span data-ttu-id="a9bb3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9bb3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9bb3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9bb3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9bb3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9bb3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9bb3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9bb3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9bb3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9bb3-115">Not supported.</span></span>|
|<span data-ttu-id="a9bb3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9bb3-116">Application</span></span>|<span data-ttu-id="a9bb3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9bb3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9bb3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9bb3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="a9bb3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9bb3-119">Request headers</span></span>
|<span data-ttu-id="a9bb3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a9bb3-120">Header</span></span>|<span data-ttu-id="a9bb3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a9bb3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9bb3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9bb3-122">Authorization</span></span>|<span data-ttu-id="a9bb3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a9bb3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9bb3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a9bb3-124">Accept</span></span>|<span data-ttu-id="a9bb3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9bb3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9bb3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9bb3-126">Request body</span></span>
<span data-ttu-id="a9bb3-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [auditEvent](../resources/intune-auditing-auditevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="a9bb3-127">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="a9bb3-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a9bb3-128">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="a9bb3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9bb3-129">Property</span></span>|<span data-ttu-id="a9bb3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a9bb3-130">Type</span></span>|<span data-ttu-id="a9bb3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9bb3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9bb3-132">id</span><span class="sxs-lookup"><span data-stu-id="a9bb3-132">id</span></span>|<span data-ttu-id="a9bb3-133">String</span><span class="sxs-lookup"><span data-stu-id="a9bb3-133">String</span></span>|<span data-ttu-id="a9bb3-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a9bb3-134">Key of the entity.</span></span>|
|<span data-ttu-id="a9bb3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a9bb3-135">displayName</span></span>|<span data-ttu-id="a9bb3-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9bb3-136">String</span></span>|<span data-ttu-id="a9bb3-137">Anzeigename des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="a9bb3-137">Event display name.</span></span>|
|<span data-ttu-id="a9bb3-138">componentName</span><span class="sxs-lookup"><span data-stu-id="a9bb3-138">componentName</span></span>|<span data-ttu-id="a9bb3-139">String</span><span class="sxs-lookup"><span data-stu-id="a9bb3-139">String</span></span>|<span data-ttu-id="a9bb3-140">Name der Komponente</span><span class="sxs-lookup"><span data-stu-id="a9bb3-140">Component name.</span></span>|
|<span data-ttu-id="a9bb3-141">actor</span><span class="sxs-lookup"><span data-stu-id="a9bb3-141">actor</span></span>|[<span data-ttu-id="a9bb3-142">auditActor</span><span class="sxs-lookup"><span data-stu-id="a9bb3-142">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="a9bb3-143">AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="a9bb3-143">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="a9bb3-144">activity</span><span class="sxs-lookup"><span data-stu-id="a9bb3-144">activity</span></span>|<span data-ttu-id="a9bb3-145">String</span><span class="sxs-lookup"><span data-stu-id="a9bb3-145">String</span></span>|<span data-ttu-id="a9bb3-146">Anzeigename der Aktivität</span><span class="sxs-lookup"><span data-stu-id="a9bb3-146">Friendly name of the activity.</span></span>|
|<span data-ttu-id="a9bb3-147">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="a9bb3-147">activityDateTime</span></span>|<span data-ttu-id="a9bb3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9bb3-148">DateTimeOffset</span></span>|<span data-ttu-id="a9bb3-149">Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format</span><span class="sxs-lookup"><span data-stu-id="a9bb3-149">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="a9bb3-150">activityType</span><span class="sxs-lookup"><span data-stu-id="a9bb3-150">activityType</span></span>|<span data-ttu-id="a9bb3-151">String</span><span class="sxs-lookup"><span data-stu-id="a9bb3-151">String</span></span>|<span data-ttu-id="a9bb3-152">Typ der durchgeführten Aktivität</span><span class="sxs-lookup"><span data-stu-id="a9bb3-152">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="a9bb3-153">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="a9bb3-153">activityOperationType</span></span>|<span data-ttu-id="a9bb3-154">String</span><span class="sxs-lookup"><span data-stu-id="a9bb3-154">String</span></span>|<span data-ttu-id="a9bb3-155">HTTP-Vorgangstyp der Aktivität</span><span class="sxs-lookup"><span data-stu-id="a9bb3-155">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="a9bb3-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="a9bb3-156">activityResult</span></span>|<span data-ttu-id="a9bb3-157">String</span><span class="sxs-lookup"><span data-stu-id="a9bb3-157">String</span></span>|<span data-ttu-id="a9bb3-158">Ergebnis der Aktivität</span><span class="sxs-lookup"><span data-stu-id="a9bb3-158">The result of the activity.</span></span>|
|<span data-ttu-id="a9bb3-159">correlationId</span><span class="sxs-lookup"><span data-stu-id="a9bb3-159">correlationId</span></span>|<span data-ttu-id="a9bb3-160">Guid</span><span class="sxs-lookup"><span data-stu-id="a9bb3-160">Guid</span></span>|<span data-ttu-id="a9bb3-161">ID der Clientanforderung, die zur Korrelation von Aktivitäten im System verwendet wird</span><span class="sxs-lookup"><span data-stu-id="a9bb3-161">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="a9bb3-162">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="a9bb3-162">resources</span></span>|<span data-ttu-id="a9bb3-163">Collection von Objekten des Typs [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="a9bb3-163">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="a9bb3-164">Ressourcen, die geändert werden</span><span class="sxs-lookup"><span data-stu-id="a9bb3-164">Resources being modified.</span></span>|
|<span data-ttu-id="a9bb3-165">Kategorie</span><span class="sxs-lookup"><span data-stu-id="a9bb3-165">category</span></span>|<span data-ttu-id="a9bb3-166">String</span><span class="sxs-lookup"><span data-stu-id="a9bb3-166">String</span></span>|<span data-ttu-id="a9bb3-167">Überwachungskategorie</span><span class="sxs-lookup"><span data-stu-id="a9bb3-167">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="a9bb3-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9bb3-168">Response</span></span>
<span data-ttu-id="a9bb3-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a9bb3-169">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9bb3-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9bb3-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9bb3-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9bb3-171">Request</span></span>
<span data-ttu-id="a9bb3-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9bb3-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
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

### <a name="response"></a><span data-ttu-id="a9bb3-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9bb3-173">Response</span></span>
<span data-ttu-id="a9bb3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9bb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




