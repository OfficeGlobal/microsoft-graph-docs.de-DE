---
title: Funktion „getManagedAppPolicies“
description: Diese Funktion ruft die App-Einschränkungen für einen bestimmten Benutzer ab.
author: tfitzmac
ms.openlocfilehash: 9b0729e986a7ab3434d2682d157e45f543d558a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354796"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="e144d-103">Funktion „getManagedAppPolicies“</span><span class="sxs-lookup"><span data-stu-id="e144d-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="e144d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e144d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e144d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e144d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e144d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e144d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e144d-107">Diese Funktion ruft die App-Einschränkungen für einen bestimmten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="e144d-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e144d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e144d-108">Prerequisites</span></span>

<span data-ttu-id="e144d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e144d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e144d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e144d-111">Permission type</span></span>|<span data-ttu-id="e144d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e144d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e144d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e144d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e144d-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="e144d-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e144d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e144d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e144d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e144d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e144d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e144d-117">Not supported.</span></span>|
|<span data-ttu-id="e144d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e144d-118">Application</span></span>|<span data-ttu-id="e144d-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e144d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e144d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e144d-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e144d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e144d-121">Request headers</span></span>

|<span data-ttu-id="e144d-122">Header</span><span class="sxs-lookup"><span data-stu-id="e144d-122">Header</span></span>|<span data-ttu-id="e144d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="e144d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e144d-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e144d-124">Authorization</span></span>|<span data-ttu-id="e144d-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e144d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e144d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e144d-126">Accept</span></span>|<span data-ttu-id="e144d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e144d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e144d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e144d-128">Request body</span></span>

<span data-ttu-id="e144d-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e144d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e144d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e144d-130">Response</span></span>

<span data-ttu-id="e144d-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e144d-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e144d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e144d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e144d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e144d-133">Request</span></span>

<span data-ttu-id="e144d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e144d-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="e144d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e144d-135">Response</span></span>

<span data-ttu-id="e144d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e144d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```






