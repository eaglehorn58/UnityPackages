# My Unity3D examples

Copyright(c) 2020, Andy Do
License type: MIT
Contact: eaglehorn58@gmail.com, eaglehorn58@163.com

---------------------------------------------
## ADQuadtreeTerrain.unitypackage

The project was made by Unity2019.3.9f1

A large-scale terrain example based on Quadtree algorithm. The example generates a 4K x 4K terrain from a raw 16-bit heightmap which can be made by terrain tools like World Machine. Bigger scale terrains can be supported without difficulty, except that more memory is required. Benefit from the Quadtree the view distance can be set very high (4K for example) without losing much perfermance. In the code Graphics.DrawProcedural method is used to do render work. Vertex and index data are stored in ComputeBuffers, no GameObject, Mesh or MeshRenderer are created, so it's also a example for how to draw custom meshes in Unity3D.

There is still a long way to go to make the little example become a completed terrain system that can be used in games, the future work may includes multithread streaming in/out data, terrain material system, collision check, etc. But if you can get some ideas or inspirations from this example, I will be very pleased.

The way to use the package:
1. Import the package into Unity3D.
2. Open the scene: Assets/ADQuadtreeTerrain/Scenes/ADQuadtreeTerrain.unity.
3. Play the game.
4. Use WASDQE keys and right button to control camera.
5. Play with the parameters on the inspector panels of QTreeTerrain and MainCamera.

![image](https://github.com/eaglehorn58/UnityPackages/tree/master/Images/QuadtreeTerrain03.jpg)
![image](https://github.com/eaglehorn58/UnityPackages/tree/master/Images/QuadtreeTerrain04.jpg)
![image](https://github.com/eaglehorn58/UnityPackages/tree/master/Images/QuadtreeTerrain05.jpg)
![image](https://github.com/eaglehorn58/UnityPackages/tree/master/Images/QuadtreeTerrain06.jpg)

---------------------------------------------
## ADTerrainStream.unitypackage

The project was made by Unity2019.2.0f1

A a simple example showing how to do streaming for custom terrain in Unity3D through .NET thread and file stream APIs. There isn't hierarchy or LOD mechanism in the simple custom terrain, but it is enough to explain the streaming process. 

The way to use the package:
1. Import the package into Unity3D.
2. Open the scene: Assets/ADTerrainStream/Scenes/TerrainStreamScene.unity
3. Select the menu item 'Tools->AD Terrain Stream' and click the 'Start' button in the popped window, this will create a 4K X 4K terrain and if succeed, a file will be generated at: Assets/ADTerrainStream/Terrain.data
4. Play the game.
5. Use WASDQE keys to move the camera and press right button to rotate it.
6. Adjust view distance on TestTerrain's inspector panel, adjust camera's speed on main camera's inspector panel.

See more:
https://eaglehorn58.wixsite.com/homepage/post/an-example-of-streaming-custom-terrain-in-unity3d

