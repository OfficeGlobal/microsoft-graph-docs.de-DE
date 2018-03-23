# <a name="assign-action"></a><span data-ttu-id="38ae3-101">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="38ae3-101">assign action</span></span>

> <span data-ttu-id="38ae3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="38ae3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38ae3-103">Diese Aktion ist noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="38ae3-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38ae3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="38ae3-104">Prerequisites</span></span>
<span data-ttu-id="38ae3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38ae3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="38ae3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38ae3-107">Permission type</span></span>|<span data-ttu-id="38ae3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38ae3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38ae3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38ae3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="38ae3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ae3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38ae3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38ae3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38ae3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38ae3-112">Not supported.</span></span>|
|<span data-ttu-id="38ae3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38ae3-113">Application</span></span>|<span data-ttu-id="38ae3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38ae3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38ae3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38ae3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="38ae3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38ae3-116">Request headers</span></span>
|<span data-ttu-id="38ae3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="38ae3-117">Header</span></span>|<span data-ttu-id="38ae3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="38ae3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38ae3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="38ae3-119">Authorization</span></span>|<span data-ttu-id="38ae3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="38ae3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="38ae3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="38ae3-121">Accept</span></span>|<span data-ttu-id="38ae3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="38ae3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38ae3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38ae3-123">Request body</span></span>
<span data-ttu-id="38ae3-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="38ae3-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="38ae3-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="38ae3-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="38ae3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38ae3-126">Property</span></span>|<span data-ttu-id="38ae3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="38ae3-127">Type</span></span>|<span data-ttu-id="38ae3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38ae3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38ae3-129">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="38ae3-129">managedEBookAssignments</span></span>|<span data-ttu-id="38ae3-130">Collection von Objekten des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="38ae3-130">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="38ae3-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="38ae3-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="38ae3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="38ae3-132">Response</span></span>
<span data-ttu-id="38ae3-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="38ae3-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="38ae3-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38ae3-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="38ae3-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38ae3-135">Request</span></span>
<span data-ttu-id="38ae3-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38ae3-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 318

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="38ae3-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="38ae3-137">Response</span></span>
<span data-ttu-id="38ae3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38ae3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



