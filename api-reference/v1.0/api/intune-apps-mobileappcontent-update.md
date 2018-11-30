---
title: Aktualisieren von „mobileAppContent“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppContent.
ms.openlocfilehash: f3e764866165c544fee7120978a0cef872f98d23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017248"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="d3726-103">Aktualisieren von „mobileAppContent“</span><span class="sxs-lookup"><span data-stu-id="d3726-103">Update mobileAppContent</span></span>

> <span data-ttu-id="d3726-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d3726-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3726-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d3726-105">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3726-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3726-106">Prerequisites</span></span>
<span data-ttu-id="d3726-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3726-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3726-109">Permission type</span></span>|<span data-ttu-id="d3726-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3726-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3726-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3726-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3726-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3726-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d3726-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3726-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3726-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3726-114">Not supported.</span></span>|
|<span data-ttu-id="d3726-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3726-115">Application</span></span>|<span data-ttu-id="d3726-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3726-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3726-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3726-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="d3726-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3726-118">Request headers</span></span>
|<span data-ttu-id="d3726-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d3726-119">Header</span></span>|<span data-ttu-id="d3726-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d3726-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3726-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3726-121">Authorization</span></span>|<span data-ttu-id="d3726-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3726-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3726-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d3726-123">Accept</span></span>|<span data-ttu-id="d3726-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d3726-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3726-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3726-125">Request body</span></span>
<span data-ttu-id="d3726-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) an.</span><span class="sxs-lookup"><span data-stu-id="d3726-126">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="d3726-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d3726-127">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="d3726-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3726-128">Property</span></span>|<span data-ttu-id="d3726-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d3726-129">Type</span></span>|<span data-ttu-id="d3726-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3726-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3726-131">id</span><span class="sxs-lookup"><span data-stu-id="d3726-131">id</span></span>|<span data-ttu-id="d3726-132">String</span><span class="sxs-lookup"><span data-stu-id="d3726-132">String</span></span>|<span data-ttu-id="d3726-133">Die Version der App-Inhalte</span><span class="sxs-lookup"><span data-stu-id="d3726-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="d3726-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3726-134">Response</span></span>
<span data-ttu-id="d3726-135">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d3726-135">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3726-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3726-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3726-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3726-137">Request</span></span>
<span data-ttu-id="d3726-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3726-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="d3726-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3726-139">Response</span></span>
<span data-ttu-id="d3726-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3726-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



