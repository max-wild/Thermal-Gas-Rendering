To generate gas images,

	1. Choose a directory for this blender scene and script
	
	2. Download and install Blender
	
	3. Open a command prompt at the scene and script's location by going to their location at file explorer
		and typing "cmd" into the navigation bar at the top
	
	4. Copy and paste this input with this template:
	
		[[blender location]] render_smoke.blend --background --python smoke_scene.py -- -o [[output location]] -r [[# of times 4 images are generated]]


		example:
			For generating 10,000 smoke images, -r would be 2,500 since there are 4 gas images per scene. 
			(10,000 / 4 = 2,500)
			
			"C:\Program Files\Blender Foundation\Blender 3.2\Blender" render_smoke.blend --background --python smoke_scene.py -- -o "C:\Users\Max\Documents\Blender\Smokes\trials\render7" -r 2500
			

		The dashes should be copied exactly as printed
	
	5. Wait for it to finish, this might take a while...
	
		note: make sure computer won't fall asleep
		
		also make sure you have not highlighted command prompt text, maybe press a random letter after 
		running has started, so that baking won't be suspended
	
Thanks
