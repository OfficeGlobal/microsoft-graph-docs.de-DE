# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="47a28-101">Funktion „getManagedAppDiagnosticStatuses“</span><span class="sxs-lookup"><span data-stu-id="47a28-101">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="47a28-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="47a28-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47a28-103">Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="47a28-103">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47a28-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47a28-104">Prerequisites</span></span>
<span data-ttu-id="47a28-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47a28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47a28-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47a28-107">Permission type</span></span>|<span data-ttu-id="47a28-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47a28-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47a28-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47a28-109">Delegated (work or school account)</span></span>| <span data-ttu-id="47a28-110">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="47a28-110">_varies by context_</span></span>|
| <span data-ttu-id="47a28-111">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="47a28-111">.mam</span></span> | <span data-ttu-id="47a28-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="47a28-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="47a28-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47a28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47a28-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47a28-114">Not supported.</span></span>|
|<span data-ttu-id="47a28-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47a28-115">Application</span></span>|<span data-ttu-id="47a28-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47a28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47a28-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47a28-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="47a28-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47a28-118">Request headers</span></span>
|<span data-ttu-id="47a28-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="47a28-119">Header</span></span>|<span data-ttu-id="47a28-120">Wert</span><span class="sxs-lookup"><span data-stu-id="47a28-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47a28-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="47a28-121">Authorization</span></span>|<span data-ttu-id="47a28-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47a28-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47a28-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="47a28-123">Accept</span></span>|<span data-ttu-id="47a28-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="47a28-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47a28-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47a28-125">Request body</span></span>
<span data-ttu-id="47a28-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="47a28-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47a28-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="47a28-127">Response</span></span>
<span data-ttu-id="47a28-128">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="47a28-128">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47a28-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47a28-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="47a28-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47a28-130">Request</span></span>
<span data-ttu-id="47a28-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47a28-131">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="47a28-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="47a28-132">Response</span></span>
<span data-ttu-id="47a28-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47a28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



