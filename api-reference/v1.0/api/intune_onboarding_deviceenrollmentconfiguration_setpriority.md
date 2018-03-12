# <a name="setpriority-action"></a><span data-ttu-id="50488-101">setPriority-Aktion</span><span class="sxs-lookup"><span data-stu-id="50488-101">setPriority action</span></span>

> <span data-ttu-id="50488-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="50488-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50488-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="50488-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50488-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50488-104">Prerequisites</span></span>
<span data-ttu-id="50488-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="50488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="50488-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50488-107">Permission type</span></span>|<span data-ttu-id="50488-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50488-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50488-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50488-109">Delegated (work or school account)</span></span>|<span data-ttu-id="50488-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50488-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50488-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50488-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50488-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50488-112">Not supported.</span></span>|
|<span data-ttu-id="50488-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50488-113">Application</span></span>|<span data-ttu-id="50488-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50488-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50488-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50488-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="50488-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50488-116">Request headers</span></span>
|<span data-ttu-id="50488-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="50488-117">Header</span></span>|<span data-ttu-id="50488-118">Wert</span><span class="sxs-lookup"><span data-stu-id="50488-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50488-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="50488-119">Authorization</span></span>|<span data-ttu-id="50488-120">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50488-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="50488-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50488-121">Accept</span></span>|<span data-ttu-id="50488-122">application/json</span><span class="sxs-lookup"><span data-stu-id="50488-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50488-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50488-123">Request body</span></span>
<span data-ttu-id="50488-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Parameters an.</span><span class="sxs-lookup"><span data-stu-id="50488-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="50488-125">Die folgende Tabelle zeigt die Parameter, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="50488-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="50488-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50488-126">Property</span></span>|<span data-ttu-id="50488-127">Typ</span><span class="sxs-lookup"><span data-stu-id="50488-127">Type</span></span>|<span data-ttu-id="50488-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50488-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50488-129">Priorität</span><span class="sxs-lookup"><span data-stu-id="50488-129">priority</span></span>|<span data-ttu-id="50488-130">Int32</span><span class="sxs-lookup"><span data-stu-id="50488-130">Int32</span></span>|<span data-ttu-id="50488-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="50488-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="50488-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="50488-132">Response</span></span>
<span data-ttu-id="50488-133">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50488-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50488-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50488-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="50488-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50488-135">Request</span></span>
<span data-ttu-id="50488-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50488-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="50488-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="50488-137">Response</span></span>
<span data-ttu-id="50488-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



