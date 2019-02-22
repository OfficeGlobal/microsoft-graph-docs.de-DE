---
title: DeviceConfigurationUserStateSummary aktualisieren
description: Aktualisieren der Eigenschaften eines deviceConfigurationUserStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4be67e51768e82a9077fe52b718f7b747152e41e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159927"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="6494b-103">DeviceConfigurationUserStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6494b-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="6494b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6494b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6494b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6494b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6494b-106">Aktualisieren der Eigenschaften eines [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6494b-106">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6494b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6494b-107">Prerequisites</span></span>
<span data-ttu-id="6494b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6494b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6494b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6494b-110">Permission type</span></span>|<span data-ttu-id="6494b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6494b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6494b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6494b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6494b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6494b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6494b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6494b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6494b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6494b-115">Not supported.</span></span>|
|<span data-ttu-id="6494b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6494b-116">Application</span></span>|<span data-ttu-id="6494b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6494b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6494b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6494b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="6494b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6494b-119">Request headers</span></span>
|<span data-ttu-id="6494b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6494b-120">Header</span></span>|<span data-ttu-id="6494b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6494b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6494b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6494b-122">Authorization</span></span>|<span data-ttu-id="6494b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6494b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6494b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6494b-124">Accept</span></span>|<span data-ttu-id="6494b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6494b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6494b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6494b-126">Request body</span></span>
<span data-ttu-id="6494b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="6494b-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="6494b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6494b-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="6494b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6494b-129">Property</span></span>|<span data-ttu-id="6494b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6494b-130">Type</span></span>|<span data-ttu-id="6494b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6494b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6494b-132">id</span><span class="sxs-lookup"><span data-stu-id="6494b-132">id</span></span>|<span data-ttu-id="6494b-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6494b-133">String</span></span>|<span data-ttu-id="6494b-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6494b-134">Key of the entity.</span></span>|
|<span data-ttu-id="6494b-135">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="6494b-135">unknownUserCount</span></span>|<span data-ttu-id="6494b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-136">Int32</span></span>|<span data-ttu-id="6494b-137">Anzahl Unbekannter Benutzer</span><span class="sxs-lookup"><span data-stu-id="6494b-137">Number of unknown users</span></span>|
|<span data-ttu-id="6494b-138">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="6494b-138">notApplicableUserCount</span></span>|<span data-ttu-id="6494b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-139">Int32</span></span>|<span data-ttu-id="6494b-140">Anzahl der nicht anwendbaren Benutzer</span><span class="sxs-lookup"><span data-stu-id="6494b-140">Number of not applicable users</span></span>|
|<span data-ttu-id="6494b-141">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="6494b-141">compliantUserCount</span></span>|<span data-ttu-id="6494b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-142">Int32</span></span>|<span data-ttu-id="6494b-143">Anzahl der kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="6494b-143">Number of compliant users</span></span>|
|<span data-ttu-id="6494b-144">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="6494b-144">remediatedUserCount</span></span>|<span data-ttu-id="6494b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-145">Int32</span></span>|<span data-ttu-id="6494b-146">Anzahl der beZahlten Benutzer</span><span class="sxs-lookup"><span data-stu-id="6494b-146">Number of remediated users</span></span>|
|<span data-ttu-id="6494b-147">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="6494b-147">nonCompliantUserCount</span></span>|<span data-ttu-id="6494b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-148">Int32</span></span>|<span data-ttu-id="6494b-149">Anzahl der nicht kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="6494b-149">Number of NonCompliant users</span></span>|
|<span data-ttu-id="6494b-150">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="6494b-150">errorUserCount</span></span>|<span data-ttu-id="6494b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-151">Int32</span></span>|<span data-ttu-id="6494b-152">Anzahl der Fehler Benutzer</span><span class="sxs-lookup"><span data-stu-id="6494b-152">Number of error users</span></span>|
|<span data-ttu-id="6494b-153">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="6494b-153">conflictUserCount</span></span>|<span data-ttu-id="6494b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-154">Int32</span></span>|<span data-ttu-id="6494b-155">Anzahl der Konflikt Benutzer</span><span class="sxs-lookup"><span data-stu-id="6494b-155">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="6494b-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="6494b-156">Response</span></span>
<span data-ttu-id="6494b-157">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6494b-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6494b-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6494b-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="6494b-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6494b-159">Request</span></span>
<span data-ttu-id="6494b-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6494b-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="6494b-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="6494b-161">Response</span></span>
<span data-ttu-id="6494b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6494b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "e8957887-7887-e895-8778-95e8877895e8",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```




