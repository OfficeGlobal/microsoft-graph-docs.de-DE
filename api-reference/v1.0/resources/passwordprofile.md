# <a name="passwordprofile-resource-type"></a><span data-ttu-id="32495-101">passwordProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="32495-101">passwordProfile resource type</span></span>

<span data-ttu-id="32495-p101">Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der [user](user.md)-Entität ist ein **asswordProfile**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="32495-p101">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="32495-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="32495-104">Properties</span></span>
| <span data-ttu-id="32495-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32495-105">Property</span></span>     | <span data-ttu-id="32495-106">Typ</span><span class="sxs-lookup"><span data-stu-id="32495-106">Type</span></span>   |<span data-ttu-id="32495-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32495-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32495-108">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="32495-108">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="32495-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="32495-109">Boolean</span></span>| <span data-ttu-id="32495-110">**true**, wenn der Benutzer sein Kennwort bei der nächsten Anmeldung ändern muss, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="32495-110">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="32495-111">password</span><span class="sxs-lookup"><span data-stu-id="32495-111">password</span></span>|<span data-ttu-id="32495-112">String</span><span class="sxs-lookup"><span data-stu-id="32495-112">String</span></span>|<span data-ttu-id="32495-p102">Das Kennwort für den Benutzer.. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Sie kann aktualisiert werden, aber der Benutzer muss das Kennwort bei der nächsten Anmeldung ändern. Das Kennwort muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft des Benutzers angegeben.  Standardmäßig ist ein sicheres Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32495-p102">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32495-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="32495-118">JSON representation</span></span>

<span data-ttu-id="32495-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="32495-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->