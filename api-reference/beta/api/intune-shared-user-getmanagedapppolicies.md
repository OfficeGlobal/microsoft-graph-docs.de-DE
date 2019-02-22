---
title: Funktion „getManagedAppPolicies“
description: Diese Funktion ruft die App-Einschränkungen für einen bestimmten Benutzer ab.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 242c640cc7d00f3c919d4823c8c93125db48ffce
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167130"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="64304-103">Funktion „getManagedAppPolicies“</span><span class="sxs-lookup"><span data-stu-id="64304-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="64304-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="64304-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64304-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64304-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64304-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="64304-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64304-107">Diese Funktion ruft die App-Einschränkungen für einen bestimmten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="64304-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64304-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="64304-108">Prerequisites</span></span>

<span data-ttu-id="64304-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64304-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="64304-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64304-111">Permission type</span></span>|<span data-ttu-id="64304-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64304-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64304-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64304-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="64304-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="64304-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="64304-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64304-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="64304-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64304-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64304-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64304-117">Not supported.</span></span>|
|<span data-ttu-id="64304-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64304-118">Application</span></span>|<span data-ttu-id="64304-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64304-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64304-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64304-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="64304-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64304-121">Request headers</span></span>

|<span data-ttu-id="64304-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="64304-122">Header</span></span>|<span data-ttu-id="64304-123">Wert</span><span class="sxs-lookup"><span data-stu-id="64304-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64304-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="64304-124">Authorization</span></span>|<span data-ttu-id="64304-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="64304-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64304-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="64304-126">Accept</span></span>|<span data-ttu-id="64304-127">application/json</span><span class="sxs-lookup"><span data-stu-id="64304-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64304-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64304-128">Request body</span></span>

<span data-ttu-id="64304-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="64304-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64304-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="64304-130">Response</span></span>

<span data-ttu-id="64304-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="64304-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64304-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64304-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="64304-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64304-133">Request</span></span>

<span data-ttu-id="64304-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64304-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="64304-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="64304-135">Response</span></span>

<span data-ttu-id="64304-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64304-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






