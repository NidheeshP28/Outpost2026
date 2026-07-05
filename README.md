# Outpost2026
Project Summary: Micro Bumper Car Drivetrain Evolution
Jul 4, 2026
Nidheesh
Nidheesh


I started by designing a miniature bumper car body with a 2x2x2-inch footprint, including a main chassis and a top cover plate secured by four screws. I set up a two-wheel differential drive system combined with a single internal front ball caster for stability, making sure the wheels and caster aligned perfectly on the floor plane.

Then, I selected a 6V, 500 RPM N20 micro gearmotor from Pololu, which has an extended rear shaft. I downloaded the official CAD files and successfully identified the correct part file to bring into my Autodesk Inventor assembly. After analyzing how the motors fit inside the tight chassis space, I realized they are too long to sit end-to-end in a straight line. I drew up a staggered layout concept with spur gears and successfully configured Inventor to generate perfectly sized micro spur gears after adjusting for imperial unit settings. To optimize space even better, I decided to pivot to a vertical motor layout where the motors stand completely upright. I used Inventor’s bevel gear generator to create a pair of tiny 90-degree gears with a perfect 1:1 ratio. I designed and made the entire internal assembly layout myself by constraining the vertical motors and interlocking the bevel gears directly to the wheel axles.

After that, I successfully imported the ball caster and modeled a dedicated, custom 3D-printable base mount platform directly on the chassis floor. Next, I realized that the wheels and axles were completely unsupported, which would cause them to sag and strip the gears under a load. I sketched an internal support tunnel on the chassis wall and overcame an extrusion direction error to successfully join the plastic inward.

Finally, I designed a custom flat-bottomed support block that connects directly to the tunnel and sits flush against the chassis floor to fully support the wheel axle, eliminate the lever arm effect, and keep my bevel gears perfectly aligned under load.

image

Inner Module Nearly Complete
Jul 4, 2026
Nidheesh
Nidheesh


I started by designing a miniature bumper car body with a 2x2x2-inch footprint, including a main chassis and a top cover plate secured by four screws. I set up a two-wheel differential drive system combined with a single internal front ball caster for stability, making sure the wheels and caster aligned perfectly on the floor plane. Then, I selected a 6V, 500 RPM N20 micro gearmotor from Pololu, which has an extended rear shaft. I downloaded the official CAD files and successfully identified the correct part file to bring into my Autodesk Inventor assembly. After analyzing how the motors fit inside the tight chassis space, I realized they are too long to sit end-to-end in a straight line. I drew up a staggered layout concept with spur gears and successfully configured Inventor to generate perfectly sized micro spur gears after adjusting for imperial unit settings. To optimize space even better, I decided to pivot to a vertical motor layout where the motors stand completely upright. I used Inventor’s bevel gear generator to create a pair of tiny 90-degree gears with a perfect 1:1 ratio. Finally, I designed and made this entire internal assembly layout myself by constraining the vertical motors and interlocking the bevel gears directly to the wheel axles. Most recently, I successfully imported the ball caster and modeled a dedicated, custom 3D-printable base mount platform directly on the chassis floor to give it a solid structural home and complete my stable, rolling drivetrain layout.

image

Completion of Drivetrain
Jul 4, 2026
Nidheesh
Nidheesh


I started by designing a miniature bumper car body with a two by two by two inch footprint including a main chassis and a top cover plate secured by four screws I set up a two wheel differential drive system combined with a single internal front ball caster for stability making sure the wheels and caster aligned perfectly on the floor plane Then I selected a six volt five hundred RPM N20 micro gearmotor from Pololu which has an extended rear shaft I downloaded the official CAD files and successfully identified the correct part file to bring into my Autodesk Inventor assembly. After analyzing how the motors fit inside the tight chassis space I realized they are too long to sit end to end in a straight line I drew up a staggered layout concept with spur gears and successfully configured Inventor to generate perfectly sized micro spur gears after adjusting for imperial unit settings. To optimize space even better I decided to pivot to a vertical motor layout where the motors stand completely upright, I used Inventor’s bevel gear generator to create a pair of tiny ninety-degree gears with a perfect one to one ratio. Finally, I designed and made this entire internal assembly layout myself by constraining the vertical motors and interlocking the bevel gears directly to the wheel axles to complete my custom high efficiency micro drivetrain.

image

Assemble W/ Motor
Jul 4, 2026
Nidheesh
Nidheesh


I started by designing a miniature bumper car body with a two by two-by-two-inch footprint including a main chassis and a top cover plate secured by four screws. I set up a two-wheel differential drive system combined with a single internal front ball caster for stability making sure the wheels and caster aligned perfectly on the floor plane. Then I selected a six volt five hundred RPM N20 micro gearmotor from Pololu which has an extended rear shaft. I downloaded the official CAD files and successfully identified the correct part file to bring into my Autodesk Inventor assembly. After analyzing how the motors fit inside the tight chassis space I realized they are too long to sit end to end in a straight line. I drew up a staggered layout concept with gears to figure out how to transfer power to the wheels and I am now deciding on the best direct drive arrangement to lock the motors into the chassis without needing extra parts.

image

Motor Identification
Jul 4, 2026
Nidheesh
Nidheesh


I started by designing a two-by-two-inch miniature bumper car body with a main chassis and a matching top cover plate. To hold the shell together securely, I added four internal corner pillars and fastened the cover plate down using four metric screws. Next, I figured out the driving mechanism for the car. I chose a differential drive layout with two independent rear wheels and a single passive ball caster sphere tucked inside the front for balance. I modeled the wheels and the front caster sphere in Inventor, cutting clean arches along the lower edge of the chassis walls so the wheels can reach the floor while aligning everything on the exact same ground plane. After evaluating motor options, I selected a high speed six volt five hundred RPM N20 micro gearmotor to give the car great power and agility. Finally, I located the exact engineering model on the Pololu website and figured out how to download the STEP file so I can bring the motor directly into my assembly.

image

Differential Drive & Pivot Steering
Jul 4, 2026
Nidheesh
Nidheesh


I started by designing a two-by-two-inch miniature bumper car body with a main chassis and a matching top cover plate. To hold the shell together securely, I added four internal corner pillars and fastened the cover plate down using four metric screws. Next, I figured out the driving mechanism for the car. I decided to go with a differential drive layout, which uses two independent rear wheels for power and steering, and a single passive ball caster sphere in the front for balance. I sketched out this layout to make sure it would fit the space perfectly. Finally, I modeled the wheels and the front caster sphere in Inventor. I cut clean semicircular arches along the lower edge of the chassis walls so the wheels can reach the floor. Right now, I have successfully aligned the wheels and the caster on the exact same ground plane, giving the car perfect clearance and leaving the frame ready for the next steps.

image

Outer Bumper Module Finished
Jul 4, 2026
Nidheesh
Nidheesh


I reviewed my assembly view to ensure the downloaded hardware matched my design layout perfectly. I imported the ISO 7380 hex socket button head screw into my project and caught a unit mismatch that originally made the screw look massive. I corrected this by changing the import units to millimeters, so it scaled down to the true size alongside my two-inch chassis. I used my engineering intuition to analyze the clearance gap between the six-millimeter screw shank and the quarter inch hole on my top cover plate. I checked the head diameter to ensure it would sit flush without overlapping the outer fillets. I updated my thread properties in Inventor by changing from imperial to the ISO Metric Profile. I configured the holes as M6 by 1 and set the behavior to full depth so the screws can pass cleanly through the pillars. I finished assembling the top cover plate onto the bumper car body with all four screws perfectly patterned, aligned, and flush against the surface.

image

Screw Identification
Jul 4, 2026
Nidheesh
Nidheesh


I evaluated my model view to find the best surfaces for starting my sketch. I confirmed that I can sketch on either the top rim of the chassis walls or the inside floor to create the corner pillars. I cleared up the math for my quarter inch top cover and quarter inch internal pillars, confirming they combine for a total depth of exactly half an inch. I planned to make the pillar holes go all the way through so that a half inch screw has extra safety clearance inside the car cavity instead of cracking the plastic. I selected the ISO 7380 hex socket button head screw. Its low-profile head keeps the top of my bumper car clean, and the hex drive provides good torque during assembly. I locked in the M3 size at 12 millimeters long, which safely fits the half inch total height while leaving a tiny safety gap at the bottom. I established the final numbers for my Inventor hole features. The top cover clearance holes will be 3.2 to 3.4 millimeters for a smooth fit, with enough flat space for the 5.7-millimeter screw head to sit flush. The pillar holes will be 2.5 millimeters so the M3 threads can bite directly into the 3D printed plastic.

image

Components Strategy
Jul 4, 2026
Nidheesh
Nidheesh


Fastener Selection & Sizing
Component Sourcing: We reviewed the metric hex nut options from the JLCMC catalog to fit your micro-scale build.

Sizing Specifications: Looked at standard vs. thin profiles for M2 and M3 hardware, identifying their widths across flats and thicknesses to ensure they fit inside your tight vertical boundaries.

CAD Tolerances: Discussed adding a $0.1 to $0.2 tolerance to 3D-printed hex pockets so the nuts can be perfectly press-fitted without cracking the plastic.

Enclosure Design Strategy
Hollow Shell Optimization: Evaluated your progress on the 3D-printed chassis, which is now a clean, hollowed-out cube with filleted exterior edges.

Internal Corner Utilization: Devised a plan to utilize the “dead space” in the four inside corners of the 2x2 footprint to create secure mounting points for top and bottom covers.3. Autodesk Inventor Workflow

Screw Bosses: Walked through the process of sketching and extruding internal corner pillars (bosses) that blend seamlessly into the interior walls without altering your smooth exterior aesthetic.

The Hole Tool: Mapped out how to implement the Hole tool to create precise pilot holes (slightly undersized for screws to tap directly into the plastic) and how to design the matching top/bottom plates with clean clearance holes.

image

The Game & Field Dimensions
Jul 4, 2026
Nidheesh
Nidheesh


The Concept: A 2v2 tabletop mechanical soccer game (similar to a real-world Rocket League).
The Field: Exactly 15×28 inches.

The Goal Wall Layout: To avoid traffic jams, you finalized a precise layout where the cars themselves frame the goal area:0.25” gap+2” car+0.25” gap+10” goal+0.25” gap+2” car+0.25” gap=15 inches

The Bumper Car Design (CAD & Hardware) The Scale: The robots are ultra-compact 2×2×2 inch cubes.
Mechanical Stack:

Bottom Layer: Two N20 gearmotors placed face-to-face right on the central axle line (so the car spins perfectly in place) with recessed wheels and a front ball caster.

Middle Layer: A 3.7V LiPo battery centered for optimal weight distribution.

Top Layer: Your custom PCB housing the microcontroller and wireless chip.

The Shell: A 2×2” protective body with a completely flat front bumper face for clean ball-striking, wrapped in an impact-absorbing foam or TPU ring.

Inventor CAD Status: We recently worked through a Loft tool error while trying to cap the roof of the car, looking at how to transition the square body into either a smooth dome or a flat recessed deck to mount your electronics.

The Electronics & Control Scheme The Controller: A custom remote featuring two joysticks.
The Drive Code: You are using a “Spin-to-Turn” control scheme. The Movement Stick handles driving straight forward and backward, while the Angle Stick spins the robot left or right in place.

Motor Mixing: The PCB’s code will use differential drive math to mix these inputs, allowing the cars to pivot on a dime or carve smooth, sweeping turns when both sticks are used together.

image

Bumper Car Module Change
Jul 4, 2026
Nidheesh
Nidheesh


Decided to change plans for the Bumper Car, since the components would fit in a spherical module, so I changed it into a cubical one

image

Bumper Car Initiation
Jul 4, 2026
Nidheesh
Nidheesh


I started to make a bumper car spherical module for the soccer board game. Here's how it looks!!!!!!

image
