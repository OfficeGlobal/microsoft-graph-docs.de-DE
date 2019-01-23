---
title: Erstellen von „auditEvent“
description: Diese Methode erstellt ein neues Objekt des Typs auditEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6f7a8bac0030b65d61e1da7fbdadfe6920b44788
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422152"
---
# <a name="create-auditevent"></a><span data-ttu-id="5d41d-103">Erstellen von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="5d41d-103">Create auditEvent</span></span>

> <span data-ttu-id="5d41d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5d41d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d41d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5d41d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d41d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d41d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d41d-107">Diese Methode erstellt ein neues Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="5d41d-107">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d41d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d41d-108">Prerequisites</span></span>
<span data-ttu-id="5d41d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d41d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5d41d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d41d-111">Permission type</span></span>|<span data-ttu-id="5d41d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d41d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d41d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d41d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d41d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d41d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d41d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d41d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d41d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d41d-116">Not supported.</span></span>|
|<span data-ttu-id="5d41d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d41d-117">Application</span></span>|<span data-ttu-id="5d41d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d41d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d41d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d41d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="5d41d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d41d-120">Request headers</span></span>
|<span data-ttu-id="5d41d-121">Header</span><span class="sxs-lookup"><span data-stu-id="5d41d-121">Header</span></span>|<span data-ttu-id="5d41d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5d41d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d41d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5d41d-123">Authorization</span></span>|<span data-ttu-id="5d41d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d41d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d41d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5d41d-125">Accept</span></span>|<span data-ttu-id="5d41d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d41d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d41d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d41d-127">Request body</span></span>
<span data-ttu-id="5d41d-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „auditEvent“ an.</span><span class="sxs-lookup"><span data-stu-id="5d41d-128">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="5d41d-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „auditEvent“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="5d41d-129">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="5d41d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d41d-130">Property</span></span>|<span data-ttu-id="5d41d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5d41d-131">Type</span></span>|<span data-ttu-id="5d41d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d41d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d41d-133">id</span><span class="sxs-lookup"><span data-stu-id="5d41d-133">id</span></span>|<span data-ttu-id="5d41d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d41d-134">String</span></span>|<span data-ttu-id="5d41d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5d41d-135">Key of the entity.</span></span>|
|<span data-ttu-id="5d41d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5d41d-136">displayName</span></span>|<span data-ttu-id="5d41d-137">String</span><span class="sxs-lookup"><span data-stu-id="5d41d-137">String</span></span>|<span data-ttu-id="5d41d-138">Anzeigename des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="5d41d-138">Event display name.</span></span>|
|<span data-ttu-id="5d41d-139">componentName</span><span class="sxs-lookup"><span data-stu-id="5d41d-139">componentName</span></span>|<span data-ttu-id="5d41d-140">String</span><span class="sxs-lookup"><span data-stu-id="5d41d-140">String</span></span>|<span data-ttu-id="5d41d-141">Name der Komponente</span><span class="sxs-lookup"><span data-stu-id="5d41d-141">Component name.</span></span>|
|<span data-ttu-id="5d41d-142">actor</span><span class="sxs-lookup"><span data-stu-id="5d41d-142">actor</span></span>|[<span data-ttu-id="5d41d-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="5d41d-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="5d41d-144">AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="5d41d-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="5d41d-145">activity</span><span class="sxs-lookup"><span data-stu-id="5d41d-145">activity</span></span>|<span data-ttu-id="5d41d-146">String</span><span class="sxs-lookup"><span data-stu-id="5d41d-146">String</span></span>|<span data-ttu-id="5d41d-147">Anzeigename der Aktivität</span><span class="sxs-lookup"><span data-stu-id="5d41d-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="5d41d-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="5d41d-148">activityDateTime</span></span>|<span data-ttu-id="5d41d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d41d-149">DateTimeOffset</span></span>|<span data-ttu-id="5d41d-150">Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format</span><span class="sxs-lookup"><span data-stu-id="5d41d-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="5d41d-151">activityType</span><span class="sxs-lookup"><span data-stu-id="5d41d-151">activityType</span></span>|<span data-ttu-id="5d41d-152">String</span><span class="sxs-lookup"><span data-stu-id="5d41d-152">String</span></span>|<span data-ttu-id="5d41d-153">Typ der durchgeführten Aktivität</span><span class="sxs-lookup"><span data-stu-id="5d41d-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="5d41d-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="5d41d-154">activityOperationType</span></span>|<span data-ttu-id="5d41d-155">String</span><span class="sxs-lookup"><span data-stu-id="5d41d-155">String</span></span>|<span data-ttu-id="5d41d-156">HTTP-Vorgangstyp der Aktivität</span><span class="sxs-lookup"><span data-stu-id="5d41d-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="5d41d-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="5d41d-157">activityResult</span></span>|<span data-ttu-id="5d41d-158">String</span><span class="sxs-lookup"><span data-stu-id="5d41d-158">String</span></span>|<span data-ttu-id="5d41d-159">Ergebnis der Aktivität</span><span class="sxs-lookup"><span data-stu-id="5d41d-159">The result of the activity.</span></span>|
|<span data-ttu-id="5d41d-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="5d41d-160">correlationId</span></span>|<span data-ttu-id="5d41d-161">Guid</span><span class="sxs-lookup"><span data-stu-id="5d41d-161">Guid</span></span>|<span data-ttu-id="5d41d-162">ID der Clientanforderung, die zur Korrelation von Aktivitäten im System verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5d41d-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="5d41d-163">resources</span><span class="sxs-lookup"><span data-stu-id="5d41d-163">resources</span></span>|<span data-ttu-id="5d41d-164">Collection von Objekten des Typs [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="5d41d-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="5d41d-165">Ressourcen, die geändert werden</span><span class="sxs-lookup"><span data-stu-id="5d41d-165">Resources being modified.</span></span>|
|<span data-ttu-id="5d41d-166">category</span><span class="sxs-lookup"><span data-stu-id="5d41d-166">category</span></span>|<span data-ttu-id="5d41d-167">String</span><span class="sxs-lookup"><span data-stu-id="5d41d-167">String</span></span>|<span data-ttu-id="5d41d-168">Überwachungskategorie</span><span class="sxs-lookup"><span data-stu-id="5d41d-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="5d41d-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d41d-169">Response</span></span>
<span data-ttu-id="5d41d-170">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [auditEvent](../resources/intune-auditing-auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5d41d-170">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d41d-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d41d-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d41d-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d41d-172">Request</span></span>
<span data-ttu-id="5d41d-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d41d-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5d41d-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d41d-174">Response</span></span>
<span data-ttu-id="5d41d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d41d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




