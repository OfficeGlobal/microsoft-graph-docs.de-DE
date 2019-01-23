---
title: WipeManagedAppRegistrationByDeviceTag Aktion
description: Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 650ff602101cead593d39603beb0b361ac0421dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415390"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="8e088-103">WipeManagedAppRegistrationByDeviceTag Aktion</span><span class="sxs-lookup"><span data-stu-id="8e088-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="8e088-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8e088-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8e088-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e088-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e088-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8e088-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e088-107">Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.</span><span class="sxs-lookup"><span data-stu-id="8e088-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e088-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e088-108">Prerequisites</span></span>

<span data-ttu-id="8e088-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e088-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e088-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e088-111">Permission type</span></span>|<span data-ttu-id="8e088-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e088-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e088-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e088-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8e088-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8e088-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8e088-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e088-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e088-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e088-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e088-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e088-117">Not supported.</span></span>|
|<span data-ttu-id="8e088-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e088-118">Application</span></span>|<span data-ttu-id="8e088-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e088-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e088-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e088-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="8e088-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e088-121">Request headers</span></span>

|<span data-ttu-id="8e088-122">Header</span><span class="sxs-lookup"><span data-stu-id="8e088-122">Header</span></span>|<span data-ttu-id="8e088-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8e088-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e088-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8e088-124">Authorization</span></span>|<span data-ttu-id="8e088-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e088-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e088-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8e088-126">Accept</span></span>|<span data-ttu-id="8e088-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8e088-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e088-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e088-128">Request body</span></span>

<span data-ttu-id="8e088-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="8e088-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8e088-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="8e088-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8e088-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e088-131">Property</span></span>|<span data-ttu-id="8e088-132">Typ</span><span class="sxs-lookup"><span data-stu-id="8e088-132">Type</span></span>|<span data-ttu-id="8e088-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e088-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e088-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8e088-134">deviceTag</span></span>|<span data-ttu-id="8e088-135">String</span><span class="sxs-lookup"><span data-stu-id="8e088-135">String</span></span>|<span data-ttu-id="8e088-136">Gerätetag</span><span class="sxs-lookup"><span data-stu-id="8e088-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="8e088-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e088-137">Response</span></span>

<span data-ttu-id="8e088-138">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="8e088-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e088-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e088-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e088-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e088-140">Request</span></span>

<span data-ttu-id="8e088-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e088-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="8e088-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e088-142">Response</span></span>

<span data-ttu-id="8e088-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e088-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






