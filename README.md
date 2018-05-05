Hello and welcome to the aircraft HUD demo and setup


Aircraft HUD will provide you a head up display like you know it from many modern aircrafts, be it private jets, fighters or helicopters.

All importat attitude information will be displayed:

Pitch
Roll
Heading
Skid or Slip
Speed and Acceleration
Altiutude and Climb speed
Flight path


Aircraft HUD is based on blueprints and materials

The Hud itself is implemented as a material that uses textures and texture masks for each indicator
By the use of Material instances  you can control the design or the display modes of the HUD

It can be used as a opaque material, that can be applied to a static mesh actor, i.e. a plane-mesh that represents one of your cockpit instruments

Or you use the HUD material in a transparent mode to paint the HUD directly on your cockpit window

If you are using a head mounted stereo display, like the Oculus rift, another feature of the Aircraft HUD will be very intresting to you : The bump offset. In bump offset Mode, the Aircraft HUD will display its information in a parallax mode, that means, the indicators will be drawn BEHIND the HUD-glass


The HUD material is controlled by a blueprint
either as a mesh
or as a UMG widget


So, If you prefer UMG Widgets for your User Interface, you can use Airrcraft HUD as a picture inside a canvas panel and display your UI 3D in the world or you can show it up on the screen space. Notice however, that you will not be able to youse the parallax mode then.

If you want to integrate the Aircraft HUD inside your project, you just have to put the Hud mes or the Hud widget component into yout pawn or actors component tree and then call an Update Event on the mesh or the widget blueprint.

The parameters you pass to the event call will update the indicators on the HUD
