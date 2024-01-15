# Computer Graphics, Winter Semester 2023

- **Name:** Your name, e.g., Maxi Musterfrau
- **E-Mail:** Your e-mail, e.g., maxi@musterfrau.de
- **Matriculation no.:** Your matriculation number: 123456789

<!--------------------------------------------------------------------------->
## Assignment 1

### Assigment 1a
The Solution:
- Vertex shader (vs): Responsible for processing individual vertices, including transformations and passing data to the fragment shader.
- Fragment shader (fs): Determines the color output for each fragment based on interpolated attributes received from the vertex shader.
The solution:
1. Adjust light position and direction in vertex shader "vs".
2. outColor is the final color output of the fragment shader so Lighting calculations are performed, including diffuse and specular reflections, to determine the final color.
### Assigment 1b
The Solution:
1. In vs: we replace the fixed values in Light position with parameters "we took those paraneters from defaultMaterial", I add those parameter to the user interface in Matierials Tab so the user can change them as he want.
2. We can also change ambient, diffuse, specular and shininess from the same interface after we add those parameters to fs shader as parameters.
3. we add "x_position,y_position,z_position" to the interface in util.js file.

### Assigment 1 Extras
<!-- Describe any extra features that you implemented. Make sure to cite your sources. -->

<!--------------------------------------------------------------------------->
## Assignment 2

### Assignment 2a
The Solution:
- To implement texture mapping we use textures (ambientMap, diffuseMap,specularMap), we will add texture coordinates parameters to "vs" and pass it to fragment shader "fs".
- Add ambientMap, diffuseMap,specularMap parameters with the texture parameter to "fs" and implement the texture in the main funcrion to get the finalcolor and the output color vector.

### Assignment 2b
The Solution:
- Calculate tangent-to-world matrix in "vs" and pass it to "fs".
- Texture the bumpMap with v_texcoord then multiply tangentToWorldMatrix with the texture and normlize it.
- use the new normalized value instead of the old one on the shape.

### Assignment 2c
The Solution:
- Add bumpIntensity, bumpFrequency and bumpAmplitude parameters and Bump function to "fs" to control bumb mapping function.
- The Bump function takes two parameters – normal (the original normal vector of the fragment) and texcoord (the texture coordinates of the fragment), It's modifies the original normal vector of a fragment by adding a sinusoidal displacement to simulate a bump mapping effect. The frequency and amplitude of the bumps can be controlled using the bumpFrequency, bumpAmplitude, and bumpIntensity parameters. Adjusting these parameters should allow us to fine-tune the appearance of the bump mapping effect on 3D model.
The 'bumpFrequency' uniform is the frequency of the sinusoidal pattern (It controls how rapidly the bumps in the surface will change, A higher frequency results in more frequent bumps), The 'bumpAmplitude' uniform represents the amplitude or height of the bumps. The bumpIntensity parameter is multiplied here to allow external control over the intensity of the bump mapping effect, Adjusting 'bumpIntensity' should make the bump effect more or less pronounced.
- Apply the function in fs main function.
- Add bumpAmplitude, bumpFrequency, and bumpIntensity to materials interface in util.js file to control the parameter.

### Assigment 2 Extras
<!-- Describe any extra features that you implemented. Make sure to cite your sources. -->

<!--------------------------------------------------------------------------->
## Assignment 3

### Assignment 3a
<!-- Briefly describe your solution. If you did not solve the assignment, simply enter "Not solved." -->

### Assignment 3b
<!-- Briefly describe your solution. If you did not solve the assignment, simply enter "Not solved." -->

### Assignment 3 Extras
<!-- Describe any extra features that you implemented. Make sure to cite your sources. -->

<!--------------------------------------------------------------------------->
## Assignment 4

### Assignment 4a
<!-- Briefly describe your solution. If you did not solve the assignment, simply enter "Not solved." -->

### Assignment 4b
<!-- Briefly describe your solution. If you did not solve the assignment, simply enter "Not solved." -->

### Assignment 4 Extras
<!-- Describe any extra features that you implemented. Make sure to cite your sources. -->