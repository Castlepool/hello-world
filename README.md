# hello-world
My first repository.

And now I made a change. I'll commit this new version in just a minute.

## Some Python Code

~~~python
def __init__(self, parentObject, acceleration=Vector((0,0,0)), 
             velocity=Vector((0,0,0)), location=Vector((0,0,0)), 
             mass=1, lifespan=10):
    # attributes, each particle needs  
    self.acceleration = acceleration
    self.velocity = velocity
    self.location = location
    self.mass = mass
    self.lifespan = lifespan
    # Object to copy from
    self.parentObject = parentObject
    # related object in 3D-space to visualize a Particle
    self.relatedObject = parentObject.copy()
    bpy.context.scene.objects.link(self.relatedObject)
    # Scale related object according to randomSize (USERINPUT)
    self.relatedObject.scale[0] = 1 + random.random() 
                                  * bpy.context.scene.randomSize
    self.relatedObject.scale[1] = 1 + random.random() 
                                  * bpy.context.scene.randomSize
    self.relatedObject.scale[2] = 1 + random.random() 
                                  * bpy.context.scene.randomSize
~~~

![Planning](Organisation_01.jpg)
