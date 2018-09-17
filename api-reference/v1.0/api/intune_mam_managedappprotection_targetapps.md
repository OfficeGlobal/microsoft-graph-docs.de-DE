# <a name="targetapps-action"></a><span data-ttu-id="410be-101">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="410be-101">targetApps action</span></span>

> <span data-ttu-id="410be-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="410be-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="410be-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="410be-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="410be-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="410be-104">Prerequisites</span></span>
<span data-ttu-id="410be-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="410be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="410be-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="410be-107">Permission type</span></span>|<span data-ttu-id="410be-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="410be-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="410be-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="410be-109">Delegated (work or school account)</span></span>|<span data-ttu-id="410be-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="410be-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="410be-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="410be-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="410be-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="410be-112">Not supported.</span></span>|
|<span data-ttu-id="410be-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="410be-113">Application</span></span>|<span data-ttu-id="410be-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="410be-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="410be-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="410be-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="410be-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="410be-116">Request headers</span></span>
|<span data-ttu-id="410be-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="410be-117">Header</span></span>|<span data-ttu-id="410be-118">Wert</span><span class="sxs-lookup"><span data-stu-id="410be-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="410be-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="410be-119">Authorization</span></span>|<span data-ttu-id="410be-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="410be-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="410be-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="410be-121">Accept</span></span>|<span data-ttu-id="410be-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="410be-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="410be-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="410be-123">Request body</span></span>
<span data-ttu-id="410be-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="410be-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="410be-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="410be-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="410be-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="410be-126">Property</span></span>|<span data-ttu-id="410be-127">Typ</span><span class="sxs-lookup"><span data-stu-id="410be-127">Type</span></span>|<span data-ttu-id="410be-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="410be-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="410be-129">Apps</span><span class="sxs-lookup"><span data-stu-id="410be-129">apps</span></span>|<span data-ttu-id="410be-130">Sammlung von Objekten des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="410be-130">[managedMobileApp](../resources/intune_mam_managedmobileapp.md) collection</span></span>|<span data-ttu-id="410be-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="410be-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="410be-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="410be-132">Response</span></span>
<span data-ttu-id="410be-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="410be-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="410be-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="410be-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="410be-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="410be-135">Request</span></span>
<span data-ttu-id="410be-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="410be-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="410be-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="410be-137">Response</span></span>
<span data-ttu-id="410be-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="410be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








