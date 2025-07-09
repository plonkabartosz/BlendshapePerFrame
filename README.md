# BlendshapePerFrame

BlendshapePerFrame is a MEL (Maya Embedded Language) script designed to automate the process of creating blendshape animations on a per-frame basis in Autodesk Maya. It allows you to automatically keyframe blendshape deformations, saving you time and effort when working with complex cloth simulations, skeletal animations, or any other animations that deform the mesh.

## Features

- **Automated keyframing:** Automatically sets blendshape values for each frame within a specified range and framerate,
- **Time-saving workflow:** Eliminates the need to manually set and key each frame,
- **Shelf integration:** An additional script (`AddToShelf.mel`) is provided to help you add the tool to your Maya shelf for quick access.

## Installation

1. **Download this repository, which includes two scripts:**
   - `BlendshapePerFrame.mel`
   - `AddToShelf.mel`

2. **Install the scripts:**
   - Copy these files into your Maya scripts directory. For example:
     - **Windows:** `C:\Users\<YourUsername>\Documents\maya\<version>\scripts\`
     - **macOS/Linux:** `~/maya/<version>/scripts/`

3. **Add to shelf (Optional):**
   - Drag and drop the `AddToShelf.mel` script inside of Maya to add a convenient shelf button that calls the BlendshapePerFrame functionality. This button allows you to launch the tool directly from Maya’s interface.

## Usage

### Prepare the scene

Make sure that you have two meshes in the scene:

1. **Animated mesh** - this mesh uses cloth simulation, is animated by a deformer, is a skinned mesh,
2. **Base mesh** - this mesh is not animated and serves as a base for the animated mesh.

### Run the script

1. **Using the script editor:**
   - Open Maya’s Script Editor,
   - Load the script, by using `File -> Open Script…`,
   - Execute the `createBlendshapeGUI()` command, to launch the script GUI.

2. **Using the shelf button:**
   - If you have used `AddToShelf.mel`, simply click the corresponding shelf button,
   - GUI will appear where you can specify:
     - **Animated/Simulated mesh:** Select a mesh that is animated/simulated,
     - **Base mesh:** Select a mesh that has no animation and where blenshapes will be created,
   - Confirm your settings and press `Create Blendshapes` to automatically create the blendshape animation.

### Review the result or adjust the settings

- **Review the animation:**
  - Play back your animation in Maya to verify that the blendshape values have been correctly applied per frame,
- **Adjust if needed:**
  - Change the playback's framerate or the range to control how many blendshapes will be created.

## License

This project and it's contents are distributed under the [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) license.

## Video Presentation

You can watch the video presentation of this script here: [artstation.com/artwork/6LxJlx](https://www.artstation.com/artwork/6LxJlx)
