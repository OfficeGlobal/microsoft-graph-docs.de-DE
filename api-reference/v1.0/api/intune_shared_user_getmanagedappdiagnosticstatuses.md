# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="688e3-101">Funktion „getManagedAppDiagnosticStatuses“</span><span class="sxs-lookup"><span data-stu-id="688e3-101">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="688e3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="688e3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="688e3-103">Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="688e3-103">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="688e3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="688e3-104">Prerequisites</span></span>
<span data-ttu-id="688e3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="688e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="688e3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="688e3-107">Permission type</span></span>|<span data-ttu-id="688e3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="688e3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="688e3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="688e3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="688e3-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="688e3-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="688e3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="688e3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="688e3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="688e3-112">Not supported.</span></span>|
|<span data-ttu-id="688e3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="688e3-113">Application</span></span>|<span data-ttu-id="688e3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="688e3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="688e3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="688e3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="688e3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="688e3-116">Request headers</span></span>
|<span data-ttu-id="688e3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="688e3-117">Header</span></span>|<span data-ttu-id="688e3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="688e3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="688e3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="688e3-119">Authorization</span></span>|<span data-ttu-id="688e3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="688e3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="688e3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="688e3-121">Accept</span></span>|<span data-ttu-id="688e3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="688e3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="688e3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="688e3-123">Request body</span></span>
<span data-ttu-id="688e3-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="688e3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="688e3-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="688e3-125">Response</span></span>
<span data-ttu-id="688e3-126">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="688e3-126">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="688e3-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="688e3-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="688e3-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="688e3-128">Request</span></span>
<span data-ttu-id="688e3-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="688e3-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="688e3-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="688e3-130">Response</span></span>
<span data-ttu-id="688e3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="688e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



