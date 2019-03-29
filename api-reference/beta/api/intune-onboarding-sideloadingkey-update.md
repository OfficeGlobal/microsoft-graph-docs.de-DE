---
title: SideLoadingKey aktualisieren
description: Aktualisieren der Eigenschaften eines sideLoadingKey-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 408cc20d76eaa06260ddd1a0de485cc3a2d57abc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977534"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="b8808-103">SideLoadingKey aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b8808-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="b8808-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8808-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8808-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8808-106">Aktualisieren der Eigenschaften eines [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8808-106">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8808-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8808-107">Prerequisites</span></span>
<span data-ttu-id="b8808-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8808-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8808-110">Permission type</span></span>|<span data-ttu-id="b8808-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8808-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8808-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8808-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8808-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8808-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b8808-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8808-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8808-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8808-115">Not supported.</span></span>|
|<span data-ttu-id="b8808-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8808-116">Application</span></span>|<span data-ttu-id="b8808-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8808-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8808-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8808-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="b8808-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8808-119">Request headers</span></span>
|<span data-ttu-id="b8808-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8808-120">Header</span></span>|<span data-ttu-id="b8808-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b8808-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8808-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8808-122">Authorization</span></span>|<span data-ttu-id="b8808-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8808-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8808-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b8808-124">Accept</span></span>|<span data-ttu-id="b8808-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8808-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8808-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8808-126">Request body</span></span>
<span data-ttu-id="b8808-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b8808-127">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="b8808-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8808-128">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="b8808-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8808-129">Property</span></span>|<span data-ttu-id="b8808-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b8808-130">Type</span></span>|<span data-ttu-id="b8808-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8808-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8808-132">id</span><span class="sxs-lookup"><span data-stu-id="b8808-132">id</span></span>|<span data-ttu-id="b8808-133">String</span><span class="sxs-lookup"><span data-stu-id="b8808-133">String</span></span>|<span data-ttu-id="b8808-134">Eindeutige ID des seitlichen Lade Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="b8808-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="b8808-135">value</span><span class="sxs-lookup"><span data-stu-id="b8808-135">value</span></span>|<span data-ttu-id="b8808-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8808-136">String</span></span>|<span data-ttu-id="b8808-137">Seiten Ladeschlüssel Wert, es ist 5x5-Wert, getrennt durch hiphens.</span><span class="sxs-lookup"><span data-stu-id="b8808-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="b8808-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b8808-138">displayName</span></span>|<span data-ttu-id="b8808-139">String</span><span class="sxs-lookup"><span data-stu-id="b8808-139">String</span></span>|<span data-ttu-id="b8808-140">Der Name des Seiten Lade Schlüssels wird den ITPro-Administratoren angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b8808-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="b8808-141">description</span><span class="sxs-lookup"><span data-stu-id="b8808-141">description</span></span>|<span data-ttu-id="b8808-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8808-142">String</span></span>|<span data-ttu-id="b8808-143">Seiten Ladeschlüssel Beschreibung, die den ITPro-Administratoren angezeigt wird..</span><span class="sxs-lookup"><span data-stu-id="b8808-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="b8808-144">totalActivation</span><span class="sxs-lookup"><span data-stu-id="b8808-144">totalActivation</span></span>|<span data-ttu-id="b8808-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b8808-145">Int32</span></span>|<span data-ttu-id="b8808-146">Die Gesamt Aktivierung des Seiten Lade Schlüssels wird den ITPro-Administratoren angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b8808-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="b8808-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8808-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="b8808-148">String</span><span class="sxs-lookup"><span data-stu-id="b8808-148">String</span></span>|<span data-ttu-id="b8808-149">Das Datum der letzten Aktualisierung, die den ITPro-Administratoren angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b8808-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="b8808-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8808-150">Response</span></span>
<span data-ttu-id="b8808-151">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8808-151">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8808-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8808-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8808-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8808-153">Request</span></span>
<span data-ttu-id="b8808-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8808-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="b8808-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8808-155">Response</span></span>
<span data-ttu-id="b8808-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8808-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```




