# item\_instance

This table holds individual item instance information for all items currently equipped in some kind of character bag or bank, in auction houses, in guild banks or in mails.

## Structure

<table>
<colgroup>
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
</colgroup>
<tbody>
<tr>
<td><p><strong>Field</strong></p></td>
<td><p><strong>Type</strong></p></td>
<td><p><strong>Attributes</strong></p></td>
<td><p><strong>Key</strong></p></td>
<td><p><strong>Null</strong></p></td>
<td><p><strong>Default</strong></p></td>
<td><p><strong>Extra</strong></p></td>
<td><p><strong>Comment</strong></p></td>
</tr>
<tr>
<td><p><a href="#guid">guid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#itementry">itemEntry</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#owner_guid">owner_guid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#creatorguid">creatorGuid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#giftcreatorguid">giftCreatorGuid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#count">count</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>1</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#duration">duration</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#charges">charges</a></p></td>
<td><p>tinytext</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>YES</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#flags">flags</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#enchantments">enchantments</a></p></td>
<td><p>text</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#randompropertyid">randomPropertyId</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#durability">durability</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#playedtime">playedTime</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#text">text</a></p></td>
<td><p>text</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>YES</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
</tbody>
</table>

## Description of the fields

### guid

The GUID of the item. This number is unique for each item instance.

### itemEntry

[Item](../world/item_template.md#entry) entry.

### owner\_guid

The GUID of the character who has ownership of this item. See [characters.guid](characters.md#guid)

### creatorGuid

[GUID](characters.md#guid) of character who created the item.

### giftCreatorGuid

[GUID](characters.md#guid) of character who created the [item](character_gifts.md#item_guid).

### count

Current number of item copies in the stack.

### duration

`field-no-description|6`

### charges

The number of charges for each of the five possible spellcharges on an item, specified via five space separated integers.

### flags

`field-no-description|8`

### enchantments

This field consists of 36 values separated by blanks. Each number is part of a 3-tuple representing an enchantment applied to the item:

1. ID in SpellItemEnchantment.dbc
2. Duration of the enchantment (optional)
3. Charges (optional)

Each of the 12 3-tuples represents a different slot for the enchantment:

1. PERM_ENCHANTMENT_SLOT

  Permanent enchantment on the item (part of the item itself).

2. TEMP_ENCHANTMENT_SLOT

  Temporary enchantments, e.g. Rogue poisons, fishing bait etc.

3. SOCK_ENCHANTMENT_SLOT
4. SOCK_ENCHANTMENT_SLOT_2
5. SOCK_ENCHANTMENT_SLOT_3

  The three slots above are related to gem sockets.

6. BONUS_ENCHANTMENT_SLOT

  Socket bonus.

7. PRISMATIC_ENCHANTMENT_SLOT

  Prismatic socket (blacksmithing).

8. PROP_ENCHANTMENT_SLOT_0
9. PROP_ENCHANTMENT_SLOT_1
10. PROP_ENCHANTMENT_SLOT_2
11. PROP_ENCHANTMENT_SLOT_3
12. PROP_ENCHANTMENT_SLOT_4

  The five slots above relate to random enchantments some items receive on creation. These slots depend either on [item_template.randomproperty](../world/item_template.md#randomproperty) or [item_template.randomsuffix](../world/item_template.md#randomsuffix).

### randomPropertyId

`field-no-description|10`

### durability

Current item durability.

### playedTime

Time in seconds

### text

The text contained in that specific item.

data-anchor=
