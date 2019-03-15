---
title: wipeManagedAppRegistrationByDeviceTag-Aktion
description: Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba8abcc4ed9b629c560c77d0c4df63f94207f242
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570668"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="b04e9-103">wipeManagedAppRegistrationByDeviceTag-Aktion</span><span class="sxs-lookup"><span data-stu-id="b04e9-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="b04e9-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="b04e9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b04e9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b04e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b04e9-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b04e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b04e9-107">Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.</span><span class="sxs-lookup"><span data-stu-id="b04e9-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b04e9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b04e9-108">Prerequisites</span></span>

<span data-ttu-id="b04e9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b04e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b04e9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b04e9-111">Permission type</span></span>|<span data-ttu-id="b04e9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b04e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b04e9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b04e9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b04e9-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="b04e9-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="b04e9-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b04e9-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b04e9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b04e9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b04e9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b04e9-117">Not supported.</span></span>|
|<span data-ttu-id="b04e9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b04e9-118">Application</span></span>|<span data-ttu-id="b04e9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b04e9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b04e9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b04e9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="b04e9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b04e9-121">Request headers</span></span>

|<span data-ttu-id="b04e9-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b04e9-122">Header</span></span>|<span data-ttu-id="b04e9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="b04e9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b04e9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b04e9-124">Authorization</span></span>|<span data-ttu-id="b04e9-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b04e9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b04e9-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b04e9-126">Accept</span></span>|<span data-ttu-id="b04e9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b04e9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b04e9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b04e9-128">Request body</span></span>

<span data-ttu-id="b04e9-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="b04e9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b04e9-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b04e9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b04e9-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b04e9-131">Property</span></span>|<span data-ttu-id="b04e9-132">Typ</span><span class="sxs-lookup"><span data-stu-id="b04e9-132">Type</span></span>|<span data-ttu-id="b04e9-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b04e9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b04e9-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="b04e9-134">deviceTag</span></span>|<span data-ttu-id="b04e9-135">String</span><span class="sxs-lookup"><span data-stu-id="b04e9-135">String</span></span>|<span data-ttu-id="b04e9-136">Gerätetag</span><span class="sxs-lookup"><span data-stu-id="b04e9-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="b04e9-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b04e9-137">Response</span></span>

<span data-ttu-id="b04e9-138">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b04e9-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b04e9-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b04e9-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b04e9-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b04e9-140">Request</span></span>

<span data-ttu-id="b04e9-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b04e9-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="b04e9-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="b04e9-142">Response</span></span>

<span data-ttu-id="b04e9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b04e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






