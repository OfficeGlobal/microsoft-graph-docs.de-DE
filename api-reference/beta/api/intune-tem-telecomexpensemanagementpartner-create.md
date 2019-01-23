---
title: telecomExpenseManagementPartner erstellen
description: Erstellen eines neuen telecomExpenseManagementPartner-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d39e3b81700b95134ea2d243f6dd8920e61f48b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395846"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="08b32-103">telecomExpenseManagementPartner erstellen</span><span class="sxs-lookup"><span data-stu-id="08b32-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="08b32-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="08b32-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="08b32-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08b32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08b32-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="08b32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08b32-107">Erstellen eines neuen [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="08b32-107">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08b32-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08b32-108">Prerequisites</span></span>
<span data-ttu-id="08b32-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="08b32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08b32-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08b32-111">Permission type</span></span>|<span data-ttu-id="08b32-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08b32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08b32-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08b32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08b32-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08b32-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08b32-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08b32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08b32-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08b32-116">Not supported.</span></span>|
|<span data-ttu-id="08b32-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08b32-117">Application</span></span>|<span data-ttu-id="08b32-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08b32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08b32-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08b32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="08b32-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08b32-120">Request headers</span></span>
|<span data-ttu-id="08b32-121">Header</span><span class="sxs-lookup"><span data-stu-id="08b32-121">Header</span></span>|<span data-ttu-id="08b32-122">Wert</span><span class="sxs-lookup"><span data-stu-id="08b32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08b32-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="08b32-123">Authorization</span></span>|<span data-ttu-id="08b32-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="08b32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08b32-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="08b32-125">Accept</span></span>|<span data-ttu-id="08b32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08b32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08b32-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08b32-127">Request body</span></span>
<span data-ttu-id="08b32-128">Geben Sie im Anforderungstext eine JSON-Darstellung des telecomExpenseManagementPartner-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="08b32-128">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="08b32-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs telecomExpenseManagementPartner erstellen.</span><span class="sxs-lookup"><span data-stu-id="08b32-129">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="08b32-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08b32-130">Property</span></span>|<span data-ttu-id="08b32-131">Typ</span><span class="sxs-lookup"><span data-stu-id="08b32-131">Type</span></span>|<span data-ttu-id="08b32-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08b32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08b32-133">id</span><span class="sxs-lookup"><span data-stu-id="08b32-133">id</span></span>|<span data-ttu-id="08b32-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08b32-134">String</span></span>|<span data-ttu-id="08b32-135">Eindeutiger Bezeichner des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="08b32-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="08b32-136">displayName</span><span class="sxs-lookup"><span data-stu-id="08b32-136">displayName</span></span>|<span data-ttu-id="08b32-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08b32-137">String</span></span>|<span data-ttu-id="08b32-138">Anzeigename des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="08b32-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="08b32-139">url</span><span class="sxs-lookup"><span data-stu-id="08b32-139">url</span></span>|<span data-ttu-id="08b32-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08b32-140">String</span></span>|<span data-ttu-id="08b32-141">Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="08b32-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="08b32-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="08b32-142">appAuthorized</span></span>|<span data-ttu-id="08b32-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="08b32-143">Boolean</span></span>|<span data-ttu-id="08b32-144">Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="08b32-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="08b32-145">enabled</span><span class="sxs-lookup"><span data-stu-id="08b32-145">enabled</span></span>|<span data-ttu-id="08b32-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="08b32-146">Boolean</span></span>|<span data-ttu-id="08b32-147">Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="08b32-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="08b32-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="08b32-148">lastConnectionDateTime</span></span>|<span data-ttu-id="08b32-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08b32-149">DateTimeOffset</span></span>|<span data-ttu-id="08b32-150">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="08b32-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="08b32-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="08b32-151">Response</span></span>
<span data-ttu-id="08b32-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="08b32-152">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08b32-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08b32-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="08b32-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08b32-154">Request</span></span>
<span data-ttu-id="08b32-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08b32-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08b32-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="08b32-156">Response</span></span>
<span data-ttu-id="08b32-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08b32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




