This is an addon for Blender 2.5+ to read/write World of warcraft's WMOs (v3.3.5).

Not all features are supported yet, mostly because the format is obviously undocumented (and some piece of data seemed unused). But most usefull features are present.
At the time I wrote this addon, it was one of the only softwares that supported creation of WMO with collisions.

The addon works as follow : 

There is 4 new panels available.
Each one contains settings used during export.

Wow WMO group panel is in Object properties, it shows options relative to wmo groups.
Group name/desc are optionnal and are just referenced from inside wmo, seems to have no effect.
This panel MUST be enabled when exporting, else export will fail.

Wow material panel is in Material properties, it shows options relative to wmo shader. The only options that are exported are shown in this panel (blender materials / texture are not exported)
Materials are displayed on faces assigned to this material.
If the panel is disabled, the material is not exported and assigned faces will not be visible in game (it can still collide though)

Wow collision panel is in Data properties and are only visible when selecting a mesh. It shows options relative to wmo collisions. "collision vertex group" specifies the vertex group whose faces will be allowed to collide.

Wow light panel is in Data properties and are only visible when selecting a lamp. It shows options relative to wmo lights. This panel will probably change later.
Lights are not exported for now.

UV
Only the active UV layer is exported. UV data imported are stored in "UVmap" layer.

Vertex color
Only the active Vertex Color layer is exported. Vertex color data imported are stored in "Col" layer.
