# Render Task
*A high-quality offline rendering of your TV show idea.* 

The theme of this work was an Alchemist/Astronomer's workspace. As such, the central idea for the scene was to create a writing desk, some clutter, and an orrery as the centerpiece.

## Models
All models were made in seperate instances of Blender. They were then copied into new blender file to create the scene. The details of their construction are as follows. No references were used.

### Brass Pentagon
The Brass Pentagon was created by simply altering the properties of a Torus object when adding it to a scene. This object mainly serves to test the creation of materials and to be used as a building block for more complex ideas. (Particularly within the unreal engine tasks) 

### Charcoal
The Charcoal was created using the cut and bevel tools to slice off the edges of an elongated cube object. 

### Inkwell
The Inkwell was create using extrude and trasform tools from a cube base. This model in particular makes use of the proportional editing mode to create a wonky object akin to a clumsily made glass bottle. It has an open top with a miniscus as well.

### Tome
The tome was made with the offset loop cut tool on a flattened and elongated cube object. The faces that would be the pages were extruded alon normals back into the book to make the hardback cover.

### Desk
The desk was made by slicing an elongated cube object into three, then elongating the two outer faces of the bottom side. Details were added to the model by cutting faces into surfaces and extruding along normals and beveling the edges.

#### Drawers
The Drawers were made using similar extrusion techniques on a shaped cube.

### Orrery
The Orrery 

#### Earth
The Earth is a UV sphere with the faces along the equator extruded along normals. An Ico Sphere, Torus, and Cylinder were added to make a brass ring and moon

#### Arm
The Arm is made up of a Brass Pentagon and two low poly cyllinders joined as one object with the centre of rotaion located at the centre of the Pentagon.

#### Sun
The Sun is comprised of a Sphere oject, a stand comprised of a Cylinder object curved outwards at the bottom using proportional editing mode. The topper is made from a a sphere, a torus, and a Cylinder that had 'To Sphere' applied.

## Materials
The Materials were mostly made in the same way. Images within the public domain and not requiring acreditation were found online and collected into a small texture library. These were then used as the base colour of the material. The colour data was then fed through a displacement node to create depth.
