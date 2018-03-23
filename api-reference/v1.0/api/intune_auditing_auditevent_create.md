# <a name="create-auditevent"></a><span data-ttu-id="7c080-101">Erstellen von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="7c080-101">Create auditEvent</span></span>

> <span data-ttu-id="7c080-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7c080-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c080-103">Diese Methode erstellt ein neues Objekt des Typs [auditEvent](../resources/intune_auditing_auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="7c080-103">Create a new [plannerBucket](../resources/intune_auditing_auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c080-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c080-104">Prerequisites</span></span>
<span data-ttu-id="7c080-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c080-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c080-107">Permission type</span></span>|<span data-ttu-id="7c080-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c080-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c080-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c080-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7c080-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c080-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c080-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c080-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c080-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c080-112">Not supported.</span></span>|
|<span data-ttu-id="7c080-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c080-113">Application</span></span>|<span data-ttu-id="7c080-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c080-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c080-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c080-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="7c080-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c080-116">Request headers</span></span>
|<span data-ttu-id="7c080-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7c080-117">Header</span></span>|<span data-ttu-id="7c080-118">Wert</span><span class="sxs-lookup"><span data-stu-id="7c080-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c080-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c080-119">Authorization</span></span>|<span data-ttu-id="7c080-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c080-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7c080-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7c080-121">Accept</span></span>|<span data-ttu-id="7c080-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7c080-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c080-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c080-123">Request body</span></span>
<span data-ttu-id="7c080-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „auditEvent“ an.</span><span class="sxs-lookup"><span data-stu-id="7c080-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="7c080-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „auditEvent“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c080-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="7c080-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c080-126">Property</span></span>|<span data-ttu-id="7c080-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7c080-127">Type</span></span>|<span data-ttu-id="7c080-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c080-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c080-129">id</span><span class="sxs-lookup"><span data-stu-id="7c080-129">id</span></span>|<span data-ttu-id="7c080-130">String</span><span class="sxs-lookup"><span data-stu-id="7c080-130">String</span></span>|<span data-ttu-id="7c080-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7c080-131">Key of the setting.</span></span>|
|<span data-ttu-id="7c080-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7c080-132">displayName</span></span>|<span data-ttu-id="7c080-133">String</span><span class="sxs-lookup"><span data-stu-id="7c080-133">String</span></span>|<span data-ttu-id="7c080-134">Anzeigename des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="7c080-134">Event display name.</span></span>|
|<span data-ttu-id="7c080-135">componentName</span><span class="sxs-lookup"><span data-stu-id="7c080-135">--componentName</span></span>|<span data-ttu-id="7c080-136">String</span><span class="sxs-lookup"><span data-stu-id="7c080-136">String</span></span>|<span data-ttu-id="7c080-137">Name der Komponente</span><span class="sxs-lookup"><span data-stu-id="7c080-137">Component name.</span></span>|
|<span data-ttu-id="7c080-138">actor</span><span class="sxs-lookup"><span data-stu-id="7c080-138">actor</span></span>|[<span data-ttu-id="7c080-139">auditActor</span><span class="sxs-lookup"><span data-stu-id="7c080-139">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="7c080-140">AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="7c080-140">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="7c080-141">activity</span><span class="sxs-lookup"><span data-stu-id="7c080-141">activity</span></span>|<span data-ttu-id="7c080-142">String</span><span class="sxs-lookup"><span data-stu-id="7c080-142">String</span></span>|<span data-ttu-id="7c080-143">Anzeigename der Aktivität</span><span class="sxs-lookup"><span data-stu-id="7c080-143">Friendly name of the activity.</span></span>|
|<span data-ttu-id="7c080-144">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="7c080-144">activityDateTime</span></span>|<span data-ttu-id="7c080-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c080-145">DateTimeOffset</span></span>|<span data-ttu-id="7c080-146">Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format</span><span class="sxs-lookup"><span data-stu-id="7c080-146">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="7c080-147">activityType</span><span class="sxs-lookup"><span data-stu-id="7c080-147">activityType</span></span>|<span data-ttu-id="7c080-148">String</span><span class="sxs-lookup"><span data-stu-id="7c080-148">String</span></span>|<span data-ttu-id="7c080-149">Typ der durchgeführten Aktivität</span><span class="sxs-lookup"><span data-stu-id="7c080-149">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="7c080-150">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="7c080-150">activityOperationType</span></span>|<span data-ttu-id="7c080-151">String</span><span class="sxs-lookup"><span data-stu-id="7c080-151">String</span></span>|<span data-ttu-id="7c080-152">HTTP-Vorgangstyp der Aktivität</span><span class="sxs-lookup"><span data-stu-id="7c080-152">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="7c080-153">activityResult</span><span class="sxs-lookup"><span data-stu-id="7c080-153">activityResult</span></span>|<span data-ttu-id="7c080-154">String</span><span class="sxs-lookup"><span data-stu-id="7c080-154">String</span></span>|<span data-ttu-id="7c080-155">Ergebnis der Aktivität</span><span class="sxs-lookup"><span data-stu-id="7c080-155">The result of the submission.</span></span>|
|<span data-ttu-id="7c080-156">correlationId</span><span class="sxs-lookup"><span data-stu-id="7c080-156">correlationId</span></span>|<span data-ttu-id="7c080-157">Guid</span><span class="sxs-lookup"><span data-stu-id="7c080-157">Guid</span></span>|<span data-ttu-id="7c080-158">ID der Clientanforderung, die zur Korrelation von Aktivitäten im System verwendet wird</span><span class="sxs-lookup"><span data-stu-id="7c080-158">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="7c080-159">resources</span><span class="sxs-lookup"><span data-stu-id="7c080-159">resources</span></span>|<span data-ttu-id="7c080-160">Collection von Objekten des Typs [auditResource](../resources/intune_auditing_auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="7c080-160">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="7c080-161">Ressourcen, die geändert werden</span><span class="sxs-lookup"><span data-stu-id="7c080-161">Resources being modified.</span></span>|
|<span data-ttu-id="7c080-162">category</span><span class="sxs-lookup"><span data-stu-id="7c080-162">category</span></span>|<span data-ttu-id="7c080-163">String</span><span class="sxs-lookup"><span data-stu-id="7c080-163">String</span></span>|<span data-ttu-id="7c080-164">Überwachungskategorie</span><span class="sxs-lookup"><span data-stu-id="7c080-164">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="7c080-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c080-165">Response</span></span>
<span data-ttu-id="7c080-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [auditEvent](../resources/intune_auditing_auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c080-166">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_auditing_auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c080-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c080-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c080-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c080-168">Request</span></span>
<span data-ttu-id="7c080-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c080-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1444

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "permissions": [
      "Permissions value"
    ],
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
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
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

### <a name="response"></a><span data-ttu-id="7c080-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c080-170">Response</span></span>
<span data-ttu-id="7c080-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c080-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1493

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "permissions": [
      "Permissions value"
    ],
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
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
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



