# areatrigger

This table contains trigger points for events in certain coordinates in the maps.

## Structure

<table>
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
<td><p><a href="#entry">entry</a></p></td>
<td><p>int (10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p>auto_increment<br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#map">map</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#x-y-and-z">x</a></p></td>
<td><p>float</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#x-y-and-z">y</a></p></td>
<td><p>float</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><a href="#x-y-and-z">z</a></td>
<td>float</td>
<td></td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><p><a href="#radius">radius</a></p></td>
<td><p>float</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#length-width-height-and-orientation">length</a></p></td>
<td><p>float</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#length-width-height-and-orientation">width</a></p></td>
<td><p>float</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#length-width-height-and-orientation">height</a></p></td>
<td><p>float</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#length-width-height-and-orientation">orientation</a></p></td>
<td><p>float</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### Entry

This is just a automatic counter that assigns a value to each trigger to list it.

### Map

The ID of the [map](../../dbc/Map.md) that the creature is spawned on.

### X, Y and Z

Contains the coordinates of the three 3d dimensions.

### Radius

This contains the radius of activation of the trigger.

### Length, Width, Height and Orientation

these fields contain the values for the physics and behavior of a given trigger.

