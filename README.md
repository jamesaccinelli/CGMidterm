# Intermediate Computer Graphics Midterm
All Textures Originate From: https://3dtextures.me/ and can be found within the Textures Folder <br>

Unity Project: 

Implementation
For a majority of the objects, I utilized Normal + Bump Mapping. This was to add realistic textures to my objects, making them feel more life-like. Normal mapping stores information such as the normal, at the uv coordinates, so we can then map 2D images to them. Bump mapping stores the height of the image, allowing us to create a 'bump' like a real life object. Additionally, I added a colour component and multiplied it within the albedo in the surf function, to match the colour of the original ship in the reference image. <br>

I also utilized Rim Lighting and Transparency to make a force field around the ship. Rim Lighting was used to create an edge of light around the outside of the object, giving us the "shield bubble" effect. This is done by taking the dot product of the normal and the normalized view direction. The transparency effect is done by using the alpha channel, and adjusting how we see through an object. This is done similarly to Rim Lighting, with the addition of taking the power of the Rim effect^transparency value. I modified this by altering the polygons used in the force field to better align with the theme of the game, hexagons -> triangles. <br>

Note:
Inputs -> 1,2 to toggle materials <br>
-> E to toggle force field
-> F to toggle camera angle
