# Particle-Motion
# Version 0.1.1 of my Particle motion program 
# Hi
    
    """(Once I get home and update the combined function due to minor changes, also I will update all the individual parts and I will simplify a few comments down and put a couple of simple .txt files that give a simple Hydrogen and two Hydrogen atoms.)"""   
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
