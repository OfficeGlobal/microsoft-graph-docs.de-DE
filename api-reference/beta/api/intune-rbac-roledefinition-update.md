---
title: roleDefinition aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs roleDefinition.
ms.openlocfilehash: debf63b5d0b7116a1e8d1f9274868d97c3cb8931
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058776"
---
# <a name="update-roledefinition"></a><span data-ttu-id="4efb6-103">roleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4efb6-103">Update roleDefinition</span></span>

> <span data-ttu-id="4efb6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4efb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4efb6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4efb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4efb6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4efb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4efb6-107">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4efb6-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4efb6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4efb6-108">Prerequisites</span></span>
<span data-ttu-id="4efb6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4efb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4efb6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4efb6-111">Permission type</span></span>|<span data-ttu-id="4efb6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4efb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4efb6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4efb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4efb6-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4efb6-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4efb6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4efb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4efb6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4efb6-116">Not supported.</span></span>|
|<span data-ttu-id="4efb6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4efb6-117">Application</span></span>|<span data-ttu-id="4efb6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4efb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4efb6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4efb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="4efb6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4efb6-120">Request headers</span></span>
|<span data-ttu-id="4efb6-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4efb6-121">Header</span></span>|<span data-ttu-id="4efb6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4efb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4efb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4efb6-123">Authorization</span></span>|<span data-ttu-id="4efb6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4efb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4efb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4efb6-125">Accept</span></span>|<span data-ttu-id="4efb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4efb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4efb6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4efb6-127">Request body</span></span>
<span data-ttu-id="4efb6-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) an.</span><span class="sxs-lookup"><span data-stu-id="4efb6-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="4efb6-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleDefinition](../resources/intune-rbac-roledefinition.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4efb6-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="4efb6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4efb6-130">Property</span></span>|<span data-ttu-id="4efb6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4efb6-131">Type</span></span>|<span data-ttu-id="4efb6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4efb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4efb6-133">id</span><span class="sxs-lookup"><span data-stu-id="4efb6-133">id</span></span>|<span data-ttu-id="4efb6-134">String</span><span class="sxs-lookup"><span data-stu-id="4efb6-134">String</span></span>|<span data-ttu-id="4efb6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4efb6-135">Key of the entity.</span></span> <span data-ttu-id="4efb6-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="4efb6-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="4efb6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4efb6-137">displayName</span></span>|<span data-ttu-id="4efb6-138">String</span><span class="sxs-lookup"><span data-stu-id="4efb6-138">String</span></span>|<span data-ttu-id="4efb6-139">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="4efb6-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="4efb6-140">description</span><span class="sxs-lookup"><span data-stu-id="4efb6-140">description</span></span>|<span data-ttu-id="4efb6-141">String</span><span class="sxs-lookup"><span data-stu-id="4efb6-141">String</span></span>|<span data-ttu-id="4efb6-142">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="4efb6-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="4efb6-143">permissions</span><span class="sxs-lookup"><span data-stu-id="4efb6-143">permissions</span></span>|<span data-ttu-id="4efb6-144">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="4efb6-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4efb6-145">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="4efb6-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4efb6-146">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="4efb6-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="4efb6-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="4efb6-147">rolePermissions</span></span>|<span data-ttu-id="4efb6-148">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="4efb6-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4efb6-149">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="4efb6-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4efb6-150">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="4efb6-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="4efb6-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4efb6-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="4efb6-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4efb6-152">Boolean</span></span>|<span data-ttu-id="4efb6-153">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="4efb6-153">Type of Role.</span></span> <span data-ttu-id="4efb6-154">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="4efb6-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="4efb6-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="4efb6-155">isBuiltIn</span></span>|<span data-ttu-id="4efb6-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4efb6-156">Boolean</span></span>|<span data-ttu-id="4efb6-157">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="4efb6-157">Type of Role.</span></span> <span data-ttu-id="4efb6-158">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="4efb6-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="4efb6-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="4efb6-159">Response</span></span>
<span data-ttu-id="4efb6-160">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4efb6-160">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4efb6-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4efb6-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="4efb6-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4efb6-162">Request</span></span>
<span data-ttu-id="4efb6-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4efb6-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1092

{
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="4efb6-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="4efb6-164">Response</span></span>
<span data-ttu-id="4efb6-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4efb6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1194

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true
}
```





