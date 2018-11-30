# Particle-Motion
# Version 1.0.2 of my Particle motion program 

    # You will need to download PYQT5 to get this progam to run as this is what I have used to create the GUI
    # You can find it here: https://sourceforge.net/projects/pyqt/
    
    """This program is once again not up to date. I need to update it and it will advance to V 1.1.0 as I put a
          skip on how often it plots to the graph because when I ran the program before it would consume all 
          the RAM in my computer without allowing me to use a long total time. It does not change how the particles
          behave because the time step does not change but it massively reduces the RAM requirements because I can
          reduce the number of lines on matplotlib by about 100x compared to the time step."""
          
    # I'm looking to add in gravity because I already have the masses in it and it will be more accurate for almost no more work.
    
    """
    This program passes info about four particles and an external Electric and Magnetic field into it from a GUI
    This program then calculates how the particles travel due to the Electric and Magnetic fields and due to interacting
        with each other over a time from t=0 to t=TotalTime.
    This program then prints the positions of the particles to the screen once every step.
        The changing Electric and Magnetic fields are taken to be independent in this simulation. A decaying Electric
        or Magnetic field does not create the other field and all velocities are taken to be much slower than the speed of light.
    Ideas for later versions include making a decaying Electric field affect the Magnetic field and vice versa. I also
        could look more into making the Relativistic calculations an option in the program as that is also quite different
        than the way the program is coded now.
    => Look up 'Relativistic Electromagnetic Potential"
    => There is a relativistic E' and B' that is given from one reference frame to another that could be used for relativistic
        potentials and allow for very high speed equations. This would most likely just add another function that would translate
        the electric and magnetic fields from frame one into frame two. Then running the forces from there.
    
    
    
    """
    """
    pos is 3x4 matrix of position
    vel is 3x4 matrix of velocity
    E0 is a matrix of strings
    B0 is a matrix of strings
    q is a 1x4 matrix
    a,b,c,d are constants
    t is looping from 0 to TotalTime by dt
    [[px1,py1,pz1],
    [px2,py2,pz2],
    [px3,py3,pz3],
    [px4,py4,pz4]]
    p stands for particle here.
    """
    """  The bondlengths ranges from the shortest of 74 pm for H-H, 74 pm = 7.4e-11 m.  """
    # http://www.science.uwaterloo.ca/~cchieh/cact/c120/bondel.html 
    # Bond distance for edge on and face on, stationary. Then futher apart with motion?
    # or rather both moving at a little further apart with a long term time scale to see effects
