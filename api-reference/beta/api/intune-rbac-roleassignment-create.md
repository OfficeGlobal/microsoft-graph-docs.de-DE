---
title: roleAssignment erstellen
description: Erstellen eines neuen roleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7bbd3624649fc576c29afaf07c532fb627d83261
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161460"
---
# <a name="create-roleassignment"></a><span data-ttu-id="49771-103">roleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="49771-103">Create roleAssignment</span></span>

> <span data-ttu-id="49771-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49771-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49771-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="49771-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49771-106">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="49771-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49771-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="49771-107">Prerequisites</span></span>
<span data-ttu-id="49771-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="49771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49771-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49771-110">Permission type</span></span>|<span data-ttu-id="49771-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49771-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49771-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49771-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49771-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49771-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="49771-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49771-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49771-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49771-115">Not supported.</span></span>|
|<span data-ttu-id="49771-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49771-116">Application</span></span>|<span data-ttu-id="49771-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49771-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49771-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49771-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="49771-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49771-119">Request headers</span></span>
|<span data-ttu-id="49771-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="49771-120">Header</span></span>|<span data-ttu-id="49771-121">Wert</span><span class="sxs-lookup"><span data-stu-id="49771-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49771-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49771-122">Authorization</span></span>|<span data-ttu-id="49771-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="49771-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49771-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="49771-124">Accept</span></span>|<span data-ttu-id="49771-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49771-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49771-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49771-126">Request body</span></span>
<span data-ttu-id="49771-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs roleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="49771-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="49771-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der roleAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="49771-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="49771-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49771-129">Property</span></span>|<span data-ttu-id="49771-130">Typ</span><span class="sxs-lookup"><span data-stu-id="49771-130">Type</span></span>|<span data-ttu-id="49771-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49771-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49771-132">id</span><span class="sxs-lookup"><span data-stu-id="49771-132">id</span></span>|<span data-ttu-id="49771-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49771-133">String</span></span>|<span data-ttu-id="49771-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="49771-134">Key of the entity.</span></span> <span data-ttu-id="49771-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="49771-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="49771-136">displayName</span><span class="sxs-lookup"><span data-stu-id="49771-136">displayName</span></span>|<span data-ttu-id="49771-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49771-137">String</span></span>|<span data-ttu-id="49771-138">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="49771-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="49771-139">description</span><span class="sxs-lookup"><span data-stu-id="49771-139">description</span></span>|<span data-ttu-id="49771-140">String</span><span class="sxs-lookup"><span data-stu-id="49771-140">String</span></span>|<span data-ttu-id="49771-141">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="49771-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="49771-142">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="49771-142">scopeMembers</span></span>|<span data-ttu-id="49771-143">String collection</span><span class="sxs-lookup"><span data-stu-id="49771-143">String collection</span></span>|<span data-ttu-id="49771-144">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="49771-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="49771-145">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="49771-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="49771-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="49771-146">scopeType</span></span>|[<span data-ttu-id="49771-147">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="49771-147">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="49771-148">Gibt den Typ des Bereichs für eine Rollenzuweisung an.</span><span class="sxs-lookup"><span data-stu-id="49771-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="49771-149">Der Standardtyp "ResourceScope" ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="49771-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="49771-150">Für "allDevices", "AllLicensedUsers" und "AllDevicesAndLicensedUsers" sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="49771-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="49771-151">Mögliche Werte: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="49771-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="49771-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="49771-152">resourceScopes</span></span>|<span data-ttu-id="49771-153">String collection</span><span class="sxs-lookup"><span data-stu-id="49771-153">String collection</span></span>|<span data-ttu-id="49771-154">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="49771-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="49771-155">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="49771-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="49771-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="49771-156">Response</span></span>
<span data-ttu-id="49771-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="49771-157">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49771-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49771-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="49771-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49771-159">Request</span></span>
<span data-ttu-id="49771-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49771-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="49771-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="49771-161">Response</span></span>
<span data-ttu-id="49771-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49771-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```




