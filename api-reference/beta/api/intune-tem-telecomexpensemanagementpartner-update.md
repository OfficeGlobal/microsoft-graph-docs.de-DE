---
title: telecomExpenseManagementPartner aktualisieren
description: Aktualisieren der Eigenschaften eines telecomExpenseManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a992a847da193ebfd799e32196a1b19b688d859a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175332"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="df483-103">telecomExpenseManagementPartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="df483-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="df483-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df483-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df483-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="df483-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df483-106">Aktualisieren der Eigenschaften eines [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="df483-106">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df483-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="df483-107">Prerequisites</span></span>
<span data-ttu-id="df483-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="df483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df483-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df483-110">Permission type</span></span>|<span data-ttu-id="df483-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df483-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df483-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df483-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df483-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df483-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df483-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df483-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df483-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df483-115">Not supported.</span></span>|
|<span data-ttu-id="df483-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df483-116">Application</span></span>|<span data-ttu-id="df483-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df483-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df483-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df483-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="df483-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df483-119">Request headers</span></span>
|<span data-ttu-id="df483-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="df483-120">Header</span></span>|<span data-ttu-id="df483-121">Wert</span><span class="sxs-lookup"><span data-stu-id="df483-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df483-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df483-122">Authorization</span></span>|<span data-ttu-id="df483-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="df483-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df483-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="df483-124">Accept</span></span>|<span data-ttu-id="df483-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df483-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df483-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df483-126">Request body</span></span>
<span data-ttu-id="df483-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="df483-127">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="df483-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="df483-128">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="df483-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df483-129">Property</span></span>|<span data-ttu-id="df483-130">Typ</span><span class="sxs-lookup"><span data-stu-id="df483-130">Type</span></span>|<span data-ttu-id="df483-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df483-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df483-132">id</span><span class="sxs-lookup"><span data-stu-id="df483-132">id</span></span>|<span data-ttu-id="df483-133">string</span><span class="sxs-lookup"><span data-stu-id="df483-133">String</span></span>|<span data-ttu-id="df483-134">Eindeutiger Bezeichner des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="df483-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="df483-135">displayName</span><span class="sxs-lookup"><span data-stu-id="df483-135">displayName</span></span>|<span data-ttu-id="df483-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df483-136">String</span></span>|<span data-ttu-id="df483-137">Anzeigename des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="df483-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="df483-138">url</span><span class="sxs-lookup"><span data-stu-id="df483-138">url</span></span>|<span data-ttu-id="df483-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df483-139">String</span></span>|<span data-ttu-id="df483-140">Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="df483-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="df483-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="df483-141">appAuthorized</span></span>|<span data-ttu-id="df483-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="df483-142">Boolean</span></span>|<span data-ttu-id="df483-143">Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="df483-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="df483-144">enabled</span><span class="sxs-lookup"><span data-stu-id="df483-144">enabled</span></span>|<span data-ttu-id="df483-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="df483-145">Boolean</span></span>|<span data-ttu-id="df483-146">Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="df483-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="df483-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="df483-147">lastConnectionDateTime</span></span>|<span data-ttu-id="df483-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df483-148">DateTimeOffset</span></span>|<span data-ttu-id="df483-149">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="df483-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="df483-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="df483-150">Response</span></span>
<span data-ttu-id="df483-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="df483-151">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df483-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df483-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="df483-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df483-153">Request</span></span>
<span data-ttu-id="df483-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df483-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="df483-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="df483-155">Response</span></span>
<span data-ttu-id="df483-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df483-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




