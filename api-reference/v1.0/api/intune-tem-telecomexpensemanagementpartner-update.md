---
title: telecomExpenseManagementPartner aktualisieren
description: Aktualisieren der Eigenschaften eines telecomExpenseManagementPartner-Objekts.
author: tfitzmac
ms.openlocfilehash: 1560a744d88da79a8b7878e03807d43e5659dd98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313916"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="e3224-103">telecomExpenseManagementPartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e3224-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="e3224-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e3224-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3224-105">Aktualisieren der Eigenschaften eines [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3224-105">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3224-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3224-106">Prerequisites</span></span>
<span data-ttu-id="e3224-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3224-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3224-109">Permission type</span></span>|<span data-ttu-id="e3224-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3224-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3224-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3224-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3224-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3224-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e3224-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3224-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3224-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3224-114">Not supported.</span></span>|
|<span data-ttu-id="e3224-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3224-115">Application</span></span>|<span data-ttu-id="e3224-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3224-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3224-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3224-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="e3224-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3224-118">Request headers</span></span>
|<span data-ttu-id="e3224-119">Header</span><span class="sxs-lookup"><span data-stu-id="e3224-119">Header</span></span>|<span data-ttu-id="e3224-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e3224-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3224-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e3224-121">Authorization</span></span>|<span data-ttu-id="e3224-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3224-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3224-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e3224-123">Accept</span></span>|<span data-ttu-id="e3224-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3224-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3224-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3224-125">Request body</span></span>
<span data-ttu-id="e3224-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e3224-126">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="e3224-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e3224-127">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="e3224-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3224-128">Property</span></span>|<span data-ttu-id="e3224-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e3224-129">Type</span></span>|<span data-ttu-id="e3224-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3224-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3224-131">id</span><span class="sxs-lookup"><span data-stu-id="e3224-131">id</span></span>|<span data-ttu-id="e3224-132">String</span><span class="sxs-lookup"><span data-stu-id="e3224-132">String</span></span>|<span data-ttu-id="e3224-133">Eindeutiger Bezeichner des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="e3224-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="e3224-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e3224-134">displayName</span></span>|<span data-ttu-id="e3224-135">String</span><span class="sxs-lookup"><span data-stu-id="e3224-135">String</span></span>|<span data-ttu-id="e3224-136">Anzeigename des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="e3224-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="e3224-137">url</span><span class="sxs-lookup"><span data-stu-id="e3224-137">url</span></span>|<span data-ttu-id="e3224-138">String</span><span class="sxs-lookup"><span data-stu-id="e3224-138">String</span></span>|<span data-ttu-id="e3224-139">Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="e3224-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="e3224-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="e3224-140">appAuthorized</span></span>|<span data-ttu-id="e3224-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e3224-141">Boolean</span></span>|<span data-ttu-id="e3224-142">Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="e3224-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="e3224-143">enabled</span><span class="sxs-lookup"><span data-stu-id="e3224-143">enabled</span></span>|<span data-ttu-id="e3224-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e3224-144">Boolean</span></span>|<span data-ttu-id="e3224-145">Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="e3224-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="e3224-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="e3224-146">lastConnectionDateTime</span></span>|<span data-ttu-id="e3224-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3224-147">DateTimeOffset</span></span>|<span data-ttu-id="e3224-148">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3224-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="e3224-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3224-149">Response</span></span>
<span data-ttu-id="e3224-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e3224-150">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3224-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3224-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3224-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3224-152">Request</span></span>
<span data-ttu-id="e3224-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3224-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="e3224-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3224-154">Response</span></span>
<span data-ttu-id="e3224-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3224-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



