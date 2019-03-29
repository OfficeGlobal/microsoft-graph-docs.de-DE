---
title: DeviceConfigurationUserStateSummary aktualisieren
description: Aktualisieren der Eigenschaften eines deviceConfigurationUserStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efc16035394ec16af3b4334df2160a176332b14a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983743"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="71906-103">DeviceConfigurationUserStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="71906-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="71906-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71906-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71906-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="71906-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71906-106">Aktualisieren der Eigenschaften eines [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71906-106">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71906-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71906-107">Prerequisites</span></span>
<span data-ttu-id="71906-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71906-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71906-110">Permission type</span></span>|<span data-ttu-id="71906-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71906-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71906-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71906-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71906-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71906-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71906-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71906-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71906-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71906-115">Not supported.</span></span>|
|<span data-ttu-id="71906-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71906-116">Application</span></span>|<span data-ttu-id="71906-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71906-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71906-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71906-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="71906-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71906-119">Request headers</span></span>
|<span data-ttu-id="71906-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71906-120">Header</span></span>|<span data-ttu-id="71906-121">Wert</span><span class="sxs-lookup"><span data-stu-id="71906-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71906-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71906-122">Authorization</span></span>|<span data-ttu-id="71906-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71906-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71906-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="71906-124">Accept</span></span>|<span data-ttu-id="71906-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71906-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71906-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71906-126">Request body</span></span>
<span data-ttu-id="71906-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="71906-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="71906-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="71906-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="71906-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71906-129">Property</span></span>|<span data-ttu-id="71906-130">Typ</span><span class="sxs-lookup"><span data-stu-id="71906-130">Type</span></span>|<span data-ttu-id="71906-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71906-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71906-132">id</span><span class="sxs-lookup"><span data-stu-id="71906-132">id</span></span>|<span data-ttu-id="71906-133">String</span><span class="sxs-lookup"><span data-stu-id="71906-133">String</span></span>|<span data-ttu-id="71906-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="71906-134">Key of the entity.</span></span>|
|<span data-ttu-id="71906-135">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="71906-135">unknownUserCount</span></span>|<span data-ttu-id="71906-136">Int32</span><span class="sxs-lookup"><span data-stu-id="71906-136">Int32</span></span>|<span data-ttu-id="71906-137">Anzahl Unbekannter Benutzer</span><span class="sxs-lookup"><span data-stu-id="71906-137">Number of unknown users</span></span>|
|<span data-ttu-id="71906-138">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="71906-138">notApplicableUserCount</span></span>|<span data-ttu-id="71906-139">Int32</span><span class="sxs-lookup"><span data-stu-id="71906-139">Int32</span></span>|<span data-ttu-id="71906-140">Anzahl der nicht anwendbaren Benutzer</span><span class="sxs-lookup"><span data-stu-id="71906-140">Number of not applicable users</span></span>|
|<span data-ttu-id="71906-141">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="71906-141">compliantUserCount</span></span>|<span data-ttu-id="71906-142">Int32</span><span class="sxs-lookup"><span data-stu-id="71906-142">Int32</span></span>|<span data-ttu-id="71906-143">Anzahl der kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="71906-143">Number of compliant users</span></span>|
|<span data-ttu-id="71906-144">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="71906-144">remediatedUserCount</span></span>|<span data-ttu-id="71906-145">Int32</span><span class="sxs-lookup"><span data-stu-id="71906-145">Int32</span></span>|<span data-ttu-id="71906-146">Anzahl der beZahlten Benutzer</span><span class="sxs-lookup"><span data-stu-id="71906-146">Number of remediated users</span></span>|
|<span data-ttu-id="71906-147">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="71906-147">nonCompliantUserCount</span></span>|<span data-ttu-id="71906-148">Int32</span><span class="sxs-lookup"><span data-stu-id="71906-148">Int32</span></span>|<span data-ttu-id="71906-149">Anzahl der nicht kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="71906-149">Number of NonCompliant users</span></span>|
|<span data-ttu-id="71906-150">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="71906-150">errorUserCount</span></span>|<span data-ttu-id="71906-151">Int32</span><span class="sxs-lookup"><span data-stu-id="71906-151">Int32</span></span>|<span data-ttu-id="71906-152">Anzahl der Fehler Benutzer</span><span class="sxs-lookup"><span data-stu-id="71906-152">Number of error users</span></span>|
|<span data-ttu-id="71906-153">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="71906-153">conflictUserCount</span></span>|<span data-ttu-id="71906-154">Int32</span><span class="sxs-lookup"><span data-stu-id="71906-154">Int32</span></span>|<span data-ttu-id="71906-155">Anzahl der Konflikt Benutzer</span><span class="sxs-lookup"><span data-stu-id="71906-155">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="71906-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="71906-156">Response</span></span>
<span data-ttu-id="71906-157">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="71906-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71906-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71906-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="71906-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71906-159">Request</span></span>
<span data-ttu-id="71906-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71906-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71906-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="71906-161">Response</span></span>
<span data-ttu-id="71906-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71906-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




