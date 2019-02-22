---
title: ManagedEBookCategory erstellen
description: Erstellen eines neuen managedEBookCategory-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd23f14bab5db4ef0d0fbae7f3ff2d752a28595c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147635"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="39565-103">ManagedEBookCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="39565-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="39565-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39565-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39565-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="39565-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39565-106">Erstellen eines neuen [managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="39565-106">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39565-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="39565-107">Prerequisites</span></span>
<span data-ttu-id="39565-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="39565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="39565-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39565-110">Permission type</span></span>|<span data-ttu-id="39565-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39565-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39565-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39565-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39565-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39565-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39565-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39565-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39565-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39565-115">Not supported.</span></span>|
|<span data-ttu-id="39565-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39565-116">Application</span></span>|<span data-ttu-id="39565-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39565-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39565-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39565-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="39565-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39565-119">Request headers</span></span>
|<span data-ttu-id="39565-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="39565-120">Header</span></span>|<span data-ttu-id="39565-121">Wert</span><span class="sxs-lookup"><span data-stu-id="39565-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39565-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="39565-122">Authorization</span></span>|<span data-ttu-id="39565-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="39565-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39565-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="39565-124">Accept</span></span>|<span data-ttu-id="39565-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39565-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39565-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39565-126">Request body</span></span>
<span data-ttu-id="39565-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das managedEBookCategory-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="39565-127">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="39565-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedEBookCategory erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="39565-128">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="39565-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="39565-129">Property</span></span>|<span data-ttu-id="39565-130">Typ</span><span class="sxs-lookup"><span data-stu-id="39565-130">Type</span></span>|<span data-ttu-id="39565-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39565-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39565-132">id</span><span class="sxs-lookup"><span data-stu-id="39565-132">id</span></span>|<span data-ttu-id="39565-133">String</span><span class="sxs-lookup"><span data-stu-id="39565-133">String</span></span>|<span data-ttu-id="39565-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="39565-134">The key of the entity.</span></span>|
|<span data-ttu-id="39565-135">displayName</span><span class="sxs-lookup"><span data-stu-id="39565-135">displayName</span></span>|<span data-ttu-id="39565-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39565-136">String</span></span>|<span data-ttu-id="39565-137">Der Name der eBook-Kategorie.</span><span class="sxs-lookup"><span data-stu-id="39565-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="39565-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39565-138">lastModifiedDateTime</span></span>|<span data-ttu-id="39565-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39565-139">DateTimeOffset</span></span>|<span data-ttu-id="39565-140">Datum und Uhrzeit der letzten Änderung des ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="39565-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="39565-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="39565-141">Response</span></span>
<span data-ttu-id="39565-142">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="39565-142">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39565-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39565-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="39565-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39565-144">Request</span></span>
<span data-ttu-id="39565-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39565-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="39565-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="39565-146">Response</span></span>
<span data-ttu-id="39565-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39565-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




