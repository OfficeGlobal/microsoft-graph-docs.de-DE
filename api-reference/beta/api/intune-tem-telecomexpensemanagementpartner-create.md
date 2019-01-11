---
title: telecomExpenseManagementPartner erstellen
description: Erstellen eines neuen telecomExpenseManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1524b8aaedfad646cfee1371a3e8529f9e60c855
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856994"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="381ff-103">telecomExpenseManagementPartner erstellen</span><span class="sxs-lookup"><span data-stu-id="381ff-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="381ff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="381ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="381ff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="381ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="381ff-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="381ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="381ff-107">Erstellen eines neuen [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="381ff-107">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="381ff-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="381ff-108">Prerequisites</span></span>
<span data-ttu-id="381ff-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="381ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="381ff-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="381ff-111">Permission type</span></span>|<span data-ttu-id="381ff-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="381ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="381ff-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="381ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="381ff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="381ff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="381ff-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="381ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="381ff-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="381ff-116">Not supported.</span></span>|
|<span data-ttu-id="381ff-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="381ff-117">Application</span></span>|<span data-ttu-id="381ff-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="381ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="381ff-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="381ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="381ff-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="381ff-120">Request headers</span></span>
|<span data-ttu-id="381ff-121">Header</span><span class="sxs-lookup"><span data-stu-id="381ff-121">Header</span></span>|<span data-ttu-id="381ff-122">Wert</span><span class="sxs-lookup"><span data-stu-id="381ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="381ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="381ff-123">Authorization</span></span>|<span data-ttu-id="381ff-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="381ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="381ff-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="381ff-125">Accept</span></span>|<span data-ttu-id="381ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="381ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="381ff-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="381ff-127">Request body</span></span>
<span data-ttu-id="381ff-128">Geben Sie im Anforderungstext eine JSON-Darstellung des telecomExpenseManagementPartner-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="381ff-128">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="381ff-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs telecomExpenseManagementPartner erstellen.</span><span class="sxs-lookup"><span data-stu-id="381ff-129">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="381ff-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="381ff-130">Property</span></span>|<span data-ttu-id="381ff-131">Typ</span><span class="sxs-lookup"><span data-stu-id="381ff-131">Type</span></span>|<span data-ttu-id="381ff-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="381ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="381ff-133">id</span><span class="sxs-lookup"><span data-stu-id="381ff-133">id</span></span>|<span data-ttu-id="381ff-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="381ff-134">String</span></span>|<span data-ttu-id="381ff-135">Eindeutiger Bezeichner des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="381ff-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="381ff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="381ff-136">displayName</span></span>|<span data-ttu-id="381ff-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="381ff-137">String</span></span>|<span data-ttu-id="381ff-138">Anzeigename des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="381ff-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="381ff-139">url</span><span class="sxs-lookup"><span data-stu-id="381ff-139">url</span></span>|<span data-ttu-id="381ff-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="381ff-140">String</span></span>|<span data-ttu-id="381ff-141">Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="381ff-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="381ff-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="381ff-142">appAuthorized</span></span>|<span data-ttu-id="381ff-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="381ff-143">Boolean</span></span>|<span data-ttu-id="381ff-144">Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="381ff-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="381ff-145">enabled</span><span class="sxs-lookup"><span data-stu-id="381ff-145">enabled</span></span>|<span data-ttu-id="381ff-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="381ff-146">Boolean</span></span>|<span data-ttu-id="381ff-147">Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="381ff-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="381ff-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="381ff-148">lastConnectionDateTime</span></span>|<span data-ttu-id="381ff-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="381ff-149">DateTimeOffset</span></span>|<span data-ttu-id="381ff-150">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="381ff-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="381ff-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="381ff-151">Response</span></span>
<span data-ttu-id="381ff-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="381ff-152">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="381ff-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="381ff-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="381ff-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="381ff-154">Request</span></span>
<span data-ttu-id="381ff-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="381ff-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
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

### <a name="response"></a><span data-ttu-id="381ff-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="381ff-156">Response</span></span>
<span data-ttu-id="381ff-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="381ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





