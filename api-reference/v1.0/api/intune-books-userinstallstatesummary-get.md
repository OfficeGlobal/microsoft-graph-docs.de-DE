---
title: Abrufen von „userInstallStateSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs userInstallStateSummary.
author: tfitzmac
ms.openlocfilehash: 4d0506b9d0e4736479d6bdd70e4176ffd82ea87c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346606"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="37647-103">Abrufen von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="37647-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="37647-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="37647-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37647-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="37647-105">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37647-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="37647-106">Prerequisites</span></span>
<span data-ttu-id="37647-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37647-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37647-109">Permission type</span></span>|<span data-ttu-id="37647-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37647-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37647-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37647-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37647-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="37647-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="37647-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37647-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37647-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37647-114">Not supported.</span></span>|
|<span data-ttu-id="37647-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37647-115">Application</span></span>|<span data-ttu-id="37647-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37647-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37647-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37647-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37647-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="37647-118">Optional query parameters</span></span>
<span data-ttu-id="37647-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="37647-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="37647-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37647-120">Request headers</span></span>
|<span data-ttu-id="37647-121">Header</span><span class="sxs-lookup"><span data-stu-id="37647-121">Header</span></span>|<span data-ttu-id="37647-122">Wert</span><span class="sxs-lookup"><span data-stu-id="37647-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37647-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="37647-123">Authorization</span></span>|<span data-ttu-id="37647-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="37647-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37647-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37647-125">Accept</span></span>|<span data-ttu-id="37647-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37647-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37647-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37647-127">Request body</span></span>
<span data-ttu-id="37647-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="37647-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37647-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="37647-129">Response</span></span>
<span data-ttu-id="37647-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="37647-130">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37647-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37647-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="37647-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37647-132">Request</span></span>
<span data-ttu-id="37647-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37647-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="37647-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="37647-134">Response</span></span>
<span data-ttu-id="37647-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37647-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```



