---
title: Erstellen von „userInstallStateSummary“
description: Diese Methode erstellt ein neues Objekt des Typs userInstallStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dbae3b5271d271a9df1215382dbf08532fd1c22
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413004"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="ae9fa-103">Erstellen von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="ae9fa-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="ae9fa-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ae9fa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae9fa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae9fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae9fa-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae9fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae9fa-107">Diese Methode erstellt ein neues Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ae9fa-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae9fa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ae9fa-108">Prerequisites</span></span>
<span data-ttu-id="ae9fa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae9fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae9fa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae9fa-111">Permission type</span></span>|<span data-ttu-id="ae9fa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae9fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae9fa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae9fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae9fa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae9fa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae9fa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae9fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae9fa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae9fa-116">Not supported.</span></span>|
|<span data-ttu-id="ae9fa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae9fa-117">Application</span></span>|<span data-ttu-id="ae9fa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae9fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae9fa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae9fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="ae9fa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae9fa-120">Request headers</span></span>
|<span data-ttu-id="ae9fa-121">Header</span><span class="sxs-lookup"><span data-stu-id="ae9fa-121">Header</span></span>|<span data-ttu-id="ae9fa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ae9fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae9fa-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ae9fa-123">Authorization</span></span>|<span data-ttu-id="ae9fa-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae9fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae9fa-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ae9fa-125">Accept</span></span>|<span data-ttu-id="ae9fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae9fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae9fa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae9fa-127">Request body</span></span>
<span data-ttu-id="ae9fa-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „userInstallStateSummary“ an.</span><span class="sxs-lookup"><span data-stu-id="ae9fa-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="ae9fa-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „userInstallStateSummary“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ae9fa-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="ae9fa-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae9fa-130">Property</span></span>|<span data-ttu-id="ae9fa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ae9fa-131">Type</span></span>|<span data-ttu-id="ae9fa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae9fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae9fa-133">id</span><span class="sxs-lookup"><span data-stu-id="ae9fa-133">id</span></span>|<span data-ttu-id="ae9fa-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae9fa-134">String</span></span>|<span data-ttu-id="ae9fa-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ae9fa-135">Key of the entity.</span></span>|
|<span data-ttu-id="ae9fa-136">userName</span><span class="sxs-lookup"><span data-stu-id="ae9fa-136">userName</span></span>|<span data-ttu-id="ae9fa-137">String</span><span class="sxs-lookup"><span data-stu-id="ae9fa-137">String</span></span>|<span data-ttu-id="ae9fa-138">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="ae9fa-138">User name.</span></span>|
|<span data-ttu-id="ae9fa-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae9fa-139">installedDeviceCount</span></span>|<span data-ttu-id="ae9fa-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ae9fa-140">Int32</span></span>|<span data-ttu-id="ae9fa-141">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="ae9fa-141">Installed Device Count.</span></span>|
|<span data-ttu-id="ae9fa-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae9fa-142">failedDeviceCount</span></span>|<span data-ttu-id="ae9fa-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ae9fa-143">Int32</span></span>|<span data-ttu-id="ae9fa-144">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="ae9fa-144">Failed Device Count.</span></span>|
|<span data-ttu-id="ae9fa-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae9fa-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="ae9fa-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ae9fa-146">Int32</span></span>|<span data-ttu-id="ae9fa-147">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="ae9fa-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="ae9fa-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae9fa-148">Response</span></span>
<span data-ttu-id="ae9fa-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ae9fa-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae9fa-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae9fa-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae9fa-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae9fa-151">Request</span></span>
<span data-ttu-id="ae9fa-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae9fa-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="ae9fa-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae9fa-153">Response</span></span>
<span data-ttu-id="ae9fa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae9fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```




