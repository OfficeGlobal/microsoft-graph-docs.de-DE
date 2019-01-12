---
title: telecomExpenseManagementPartner erstellen
description: Erstellen eines neuen telecomExpenseManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ca3a94da0c908bec0af44075dcb15b6fa4f007a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984801"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="5a708-103">telecomExpenseManagementPartner erstellen</span><span class="sxs-lookup"><span data-stu-id="5a708-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="5a708-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5a708-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a708-105">Erstellen eines neuen [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a708-105">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a708-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5a708-106">Prerequisites</span></span>
<span data-ttu-id="5a708-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a708-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a708-109">Permission type</span></span>|<span data-ttu-id="5a708-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a708-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a708-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a708-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a708-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a708-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5a708-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a708-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a708-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a708-114">Not supported.</span></span>|
|<span data-ttu-id="5a708-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a708-115">Application</span></span>|<span data-ttu-id="5a708-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a708-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a708-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a708-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="5a708-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a708-118">Request headers</span></span>
|<span data-ttu-id="5a708-119">Header</span><span class="sxs-lookup"><span data-stu-id="5a708-119">Header</span></span>|<span data-ttu-id="5a708-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5a708-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a708-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a708-121">Authorization</span></span>|<span data-ttu-id="5a708-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5a708-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a708-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5a708-123">Accept</span></span>|<span data-ttu-id="5a708-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a708-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a708-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a708-125">Request body</span></span>
<span data-ttu-id="5a708-126">Geben Sie im Anforderungstext eine JSON-Darstellung des telecomExpenseManagementPartner-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5a708-126">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="5a708-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs telecomExpenseManagementPartner erstellen.</span><span class="sxs-lookup"><span data-stu-id="5a708-127">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="5a708-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a708-128">Property</span></span>|<span data-ttu-id="5a708-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5a708-129">Type</span></span>|<span data-ttu-id="5a708-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a708-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a708-131">id</span><span class="sxs-lookup"><span data-stu-id="5a708-131">id</span></span>|<span data-ttu-id="5a708-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a708-132">String</span></span>|<span data-ttu-id="5a708-133">Eindeutiger Bezeichner des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="5a708-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="5a708-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5a708-134">displayName</span></span>|<span data-ttu-id="5a708-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a708-135">String</span></span>|<span data-ttu-id="5a708-136">Anzeigename des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="5a708-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="5a708-137">url</span><span class="sxs-lookup"><span data-stu-id="5a708-137">url</span></span>|<span data-ttu-id="5a708-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a708-138">String</span></span>|<span data-ttu-id="5a708-139">Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="5a708-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="5a708-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="5a708-140">appAuthorized</span></span>|<span data-ttu-id="5a708-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5a708-141">Boolean</span></span>|<span data-ttu-id="5a708-142">Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="5a708-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="5a708-143">enabled</span><span class="sxs-lookup"><span data-stu-id="5a708-143">enabled</span></span>|<span data-ttu-id="5a708-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5a708-144">Boolean</span></span>|<span data-ttu-id="5a708-145">Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="5a708-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="5a708-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="5a708-146">lastConnectionDateTime</span></span>|<span data-ttu-id="5a708-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a708-147">DateTimeOffset</span></span>|<span data-ttu-id="5a708-148">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a708-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="5a708-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a708-149">Response</span></span>
<span data-ttu-id="5a708-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5a708-150">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a708-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a708-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a708-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a708-152">Request</span></span>
<span data-ttu-id="5a708-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a708-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
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

### <a name="response"></a><span data-ttu-id="5a708-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a708-154">Response</span></span>
<span data-ttu-id="5a708-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a708-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



