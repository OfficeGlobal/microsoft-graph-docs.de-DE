---
title: Benutzer abrufen
description: Lesen von Eigenschaften und Beziehungen des user-Objekts.
author: tfitzmac
ms.openlocfilehash: cf0ee7b2c6d9cf13176f65c174ee4b6ac986984b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359689"
---
# <a name="get-user"></a><span data-ttu-id="29592-103">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="29592-103">Get user</span></span>

> <span data-ttu-id="29592-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="29592-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29592-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="29592-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29592-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="29592-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29592-107">Lesen von Eigenschaften und Beziehungen des [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="29592-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29592-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="29592-108">Prerequisites</span></span>

<span data-ttu-id="29592-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="29592-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="29592-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29592-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="29592-111">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="29592-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="29592-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29592-112">Permission type</span></span>|<span data-ttu-id="29592-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29592-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29592-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29592-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="29592-115">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="29592-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="29592-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="29592-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="29592-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="29592-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="29592-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="29592-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="29592-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="29592-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="29592-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29592-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="29592-121">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="29592-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="29592-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="29592-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="29592-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29592-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29592-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29592-124">Not supported.</span></span>|
|<span data-ttu-id="29592-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29592-125">Application</span></span>|<span data-ttu-id="29592-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29592-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29592-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29592-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29592-128">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="29592-128">Optional query parameters</span></span>

<span data-ttu-id="29592-129">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29592-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29592-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29592-130">Request headers</span></span>

|<span data-ttu-id="29592-131">Header</span><span class="sxs-lookup"><span data-stu-id="29592-131">Header</span></span>|<span data-ttu-id="29592-132">Wert</span><span class="sxs-lookup"><span data-stu-id="29592-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29592-133">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="29592-133">Authorization</span></span>|<span data-ttu-id="29592-134">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="29592-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29592-135">Accept</span><span class="sxs-lookup"><span data-stu-id="29592-135">Accept</span></span>|<span data-ttu-id="29592-136">application/json</span><span class="sxs-lookup"><span data-stu-id="29592-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29592-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29592-137">Request body</span></span>

<span data-ttu-id="29592-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="29592-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29592-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="29592-139">Response</span></span>

<span data-ttu-id="29592-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/intune-shared-user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29592-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29592-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29592-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="29592-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29592-142">Request</span></span>

<span data-ttu-id="29592-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29592-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="29592-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="29592-144">Response</span></span>

<span data-ttu-id="29592-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29592-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



